<script lang="ts">
  export let level: any
  export let records: any

  let record: any;

  $: handleLevelChange(level);
  
  function handleLevelChange(level: number) {
    record = records.find((value: any) => {
      return value.level === level
    })
    console.log('record', record)
  }
</script>

<div class="container">
  <h1 class="title">Pricing</h1>
  <h2 class="description">Level: {level}</h2>
  <form action="#">
    <p class="range-field">
      <input type="range" id="pricing-slider" min="0" max="10" bind:value={level} />
    </p>
  </form>
  {#if record}
    <div>At this pricing level subscribers may keep unlimited records, store {record.storage} GB of data, and make {record.requestsPerMonth.toLocaleString("en-US")} API requests per month; all of which will cost the owner ${(record.price).toLocaleString("en-US")} per month.</div>
  {/if}
  <br />
  <div class="card z-depth-5">
    <div class="row" style="margin: 0;">
      <div class="col s6">
        <div class="card-content">
          <div class="card-title">Start a Trial:</div>
          Test every feature in subvind free forever. Some usage limits apply.
          <br /><br />
          <a href="https://client-area.istrav.com" class="btn transparent black-text">Start Your Trial</a>
          <br /><div style="margin-top: 1em; color: #888;">No credit card required.</div>
        </div>
      </div>
      <div class="col s6 demo">
        <div class="card-content">
          <div class="card-title">Grab a Demo:</div>
          For a one-on-one walk-through of subvind with an in-house expert please contact us. 
          <br />
          <br />
          <a href="https://demo.subvind.com" target="_blank" class="btn red lighten-2">Goto Demo</a>
          <br />
          <br />
          <br />
        </div>
      </div>
    </div>
    <div class="card-action">
      <div class="row" style="margin: 0;">
        <div class="col s4">
          <ul class="collection">
            <li class="collection-item"><i class="material-icons">check</i> Unlimited accounts</li>
            <li class="collection-item"><i class="material-icons">check</i> Unlimited products</li>
            <li class="collection-item"><i class="material-icons">check</i> Unlimited inventory</li>
            <li class="collection-item"><i class="material-icons">check</i> Unlimited orders</li>
          </ul>
        </div>
        <div class="col s4">
          <ul class="collection">
            <li class="collection-item"><i class="material-icons">check</i> SSL encryption for security</li>
            <li class="collection-item"><i class="material-icons">check</i> 3rd Party Integrations</li>
            <li class="collection-item"><i class="material-icons">check</i> Headless API</li>
            <li class="collection-item"><i class="material-icons">check</i> Bolt-on Modules</li>
          </ul>
        </div>
        <div class="col s4">
          <ul class="collection">
            <li class="collection-item"><i class="material-icons">check</i> Micro Software as a Service</li>
            <li class="collection-item"><i class="material-icons">check</i> Monolithic Back-End</li>
            <li class="collection-item"><i class="material-icons">check</i> White Labeled</li>
            <li class="collection-item"><i class="material-icons">check</i> Fully Customizable</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</div>

<style>
	.title {
		font-weight: 900;
		font-size: 4.5em;
		text-align: left;
		margin: 0;
	}

  .description {
    color: #000;
    font-size: 2.5em;
    margin: 0;
  }

  #pricing-slider {
    border: 0;
  }
	.demo {
		background: #26a69a;
    color: #fff;
	}

  .card-action {
    background: #eee;
    padding: 0.5em 0 0;
  }

  .collection {
    border: 1px solid #aaa;
    border-bottom: 0;
  }
  .collection .collection-item {
    border-bottom: 1px solid #aaa;
    background: #ddd;
    display: flex;
    align-items: center;
  }
  .collection .collection-item i {
    color: #26a69a;
  }
</style>