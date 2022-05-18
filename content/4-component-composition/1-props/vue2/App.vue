<script>
import UserProfile from './UserProfile.vue';
export default {
	components: { UserProfile },
};
</script>

<template>
  <UserProfile
    name="John"
    :age="20"
    :favourite-colors="['green', 'blue', 'red']"
    is-available
  />
</template>
