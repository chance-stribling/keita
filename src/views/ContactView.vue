<script setup></script>

<template>
  <div class="main">
    <div class="content">
        <div action="">
            <label for="fname">First Name</label>
            <input type="text" id="fname" name="firstname" placeholder="Your name..">

            <label for="lname">Last Name</label>
            <input type="text" id="lname" name="lastname" placeholder="Your last name..">

            <label for="country">Country</label>
            <select id="country" name="country">
            <option value="australia">Australia</option>
            <option value="canada">Canada</option>
            <option value="usa">USA</option>
            </select>

            <label for="subject">Subject</label>
            <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea>

            <input type="submit" value="Submit">
        </div>
    </div>
  </div>
</template>
<style scoped>
.main {
  display: flex;
  flex-direction: column;
  align-items: end;
  justify-content: end;
  height: 100%;
  padding: 2rem;
  color: white;
}
.content {
  width: 150px;
}
.text{
  font-size: 16px;
}
</style>
