<script lang="ts">
    import {user, userData} from "$lib/firebase"
  
    $user;
    $userData;
  </script>

  <div class="min-h-screen flex flex-col">
    <slot />
  </div>