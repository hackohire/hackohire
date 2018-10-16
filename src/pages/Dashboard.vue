<template>
  <b-container>
    <div class="b-main-content">
    <ul class="list-inline">
          <li class="list-inline-item">
            <a href="/profile">Profile</a>
          </li>
          <li class="list-inline-item">
            <a href="#">Jobs</a>
          </li>
          <li class="list-inline-item">
            <a href="#">Mentors</a>
          </li>
        </ul>
      <h2>Welcome to hackohire</h2>
      <p>{{ user.username }}, Thank you for requesting the trial access.</p>
    </div> 
  </b-container> 
</template>

<script>
import { mapState } from 'vuex'

export default {
    computed: {
        ...mapState({
            user: state => state.auth.user,
        })
    }
}
</script>

