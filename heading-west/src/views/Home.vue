<template>
    <span>
        <home-back></home-back>
        <west-details></west-details>
        <west-engagements></west-engagements>
    </span>
</template>

<script>
import homeBack from '@/components/homeBack';
import westDetails from '@/components/westDetails';
import westEngagements from '@/components/westEngagements';

export default {
    name: 'home',
    components: {
        homeBack,
        westDetails,
        westEngagements
    }
};
</script>
