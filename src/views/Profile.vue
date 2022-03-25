<template>
<div id="app" class="modal-vue">
<!-- Modal -->
<div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel">Edit Profile</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>

      <div class="modal-body">
        <div class="img-center"><br>
        <!-- <img src="../assets/Logo.png" alt="Avatar" style="width:30%" class="avatar"> -->
      </div><br><br>
      <form class="container">
        <div class="section">
          <label><b>Username</b></label><br>
          <input class="input border margin-bottom" type="text" placeholder="Enter Username" name="usrname" required><br><br>
          <label><b>Password</b></label><br>
          <input class="input border" type="password" placeholder="Enter Password" name="pass" required><br>
          <button class="button block green section padding" type="submit">Login</button><br>
          <input class="check margin-top" type="checkbox" checked="checked"> Remember me
        </div>
      </form>
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Save changes</button>
      </div>
    </div>
  </div>
</div> 
</div>
</template>

<script>
export default {
}
</script>

<style>

</style>