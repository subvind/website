
<div class="container">
  <a href="/resume">
    <div class="get-started-now">
      <h1 style="text-align: center; margin-top: 0; font-weight: 900;">Custom Work:</h1>
      <h4 style="text-align: center; margin-top: -0.5em;">Full Stack Developer<br /> starting at $80/hour</h4>
    </div>
  </a>
</div>

<style>
  .container {
    width: 100%;
    max-width: 900px;
    margin: 0 auto;
  }

  .get-started-now {
    /* background: #E57373; */
    max-width: 80%;
    padding: 1em;
    margin: 0 auto;
    position: relative;
    color: #fff;
  }
  
  .get-started-now:before {
    background-color: #42a5f5;
    transform: skewy(1deg); /* angle you want */
    transform-origin: bottom left;
    content: ' ';
    display: block;
    height: 100%;
    width: 100%;
    position: absolute;
    z-index: -1;
    top: 0;
  }

  .get-started-now:after {
    background-color: #42a5f5;
    transform: skewy(-1deg); /* angle you want */
    transform-origin: bottom left;
    border-bottom: 30px solid #42a5f5; /* bottom border skews with the object */
    content: ' ';
    display: block;
    height: 100%;
    width: 100%;
    position: absolute;
    z-index: -1;
    bottom: 0;
  }
</style>