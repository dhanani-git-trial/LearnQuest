<script>
  import "$css/index.css";
  import LearnQuest_Logo from '$images/LearnQuest_logo.png';
  function redirect() {
    location.replace('/Register');
  }
</script>
<form class="form" method="POST" autocomplete="off">
  <img height="90" width="300" alt="LearnQuest Logo" src={LearnQuest_Logo}/>
  <div class="flex-column">
    <label for="email_input">Email</label>
  </div>
  <div class="inputForm">
      <svg height="20" viewBox="0 0 32 32" width="20" xmlns="http://www.w3.org/2000/svg">
          <g id="Layer_3" data-name="Layer 3">
              <path d="M30.853 13.87a15 15 0 0 0-29.729 4.082 15.1 15.1 0 0 0 12.876 12.918 15.6 15.6 0 0 0 2.016.13 14.85 14.85 0 0 0 7.715-2.145 1 1 0 1 0-1.031-1.711 13.007 13.007 0 1 1 5.458-6.529 2.149 2.149 0 0 1-4.158-.759v-10.856a1 1 0 0 0-2 0v1.726a8 8 0 1 0 .2 10.325 4.135 4.135 0 0 0 7.83.274 15.2 15.2 0 0 0 .823-7.455zM16 22a6 6 0 1 1 6-6 6.006 6.006 0 0 1-6 6z"></path>
          </g>
      </svg>
      <input type="email" id="email_input" name="email" class="input" placeholder="Enter your Email">
  </div>

  <div class="flex-column">
    <label for="password_input">Password</label>
  </div>
  <div class="inputForm">
      <svg height="20" viewBox="-64 0 512 512" width="20" xmlns="http://www.w3.org/2000/svg">
          <path d="M336 512H48c-26.453 0-48-21.523-48-48V240c0-26.476 21.547-48 48-48h288c26.453 0 48 21.523 48 48v224c0 26.476-21.547 48-48 48zM48 224c-8.813 0-16 7.168-16 16v224c0 8.832 7.187 16 16 16h288c8.813 0 16-7.168 16-16V240c0-8.832-7.187-16-16-16z"></path>
          <path d="M304 224c-8.832 0-16-7.168-16-16v-80c0-52.93-43.07-96-96-96s-96 43.07-96 96v80c0 8.832-7.168 16-16 16s-16-7.168-16-16v-80c0-70.594 57.406-128 128-128s128 57.406 128 128v80c0 8.832-7.168 16-16 16z"></path>
      </svg>        
      <input type="password" id="password_input" name="password" class="input" placeholder="Enter your Password">
  </div>

  <div class="flex-column">
    <label>Full Name </label>
</div>
<div class="inputForm">
    <input type="text" id="name_input" name="name" class="input" placeholder="Enter your Full Name">
</div>

<div class="flex-column">
    <label>What is your mother's name?</label>
</div>
<div class="inputForm">
    <input type="tel" class="input" placeholder="Write and remember your answer.">
</div>


<div class="flex-column">
  <label>What language do you speak?</label>
</div>
<div class="inputForm">
  <input type="tel" class="input" placeholder="Write and remember your answer.">
</div>

  <button class="button-submit">Sign Up</button>
  <p class="p">Don't have an account? <span class="span" on:click={redirect}>Sign Up</span></p>
</form>
