<template>
  <div>
    <div class="intro">
        {{this.days[this.day]}} {{this.months[this.month]}} {{this.date}}
    </div>
  </div>
</template>

<script>
export default {
    name: 'Intro',
    data: function() {
        return {
            day: 0,
            month: 0,
            date: 0,
            days: ['Sunday', 'Monday','Tuesday','Wednesday','Thursday','Friday','Saturday'],
            months: ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"]
        }
    },
    created() {
        let d = new Date();
        this.day = d.getDay();
        this.month = d.getMonth();
        this.date = d.getDate();
    }
}
</script>

<style scoped>
.intro {
    color: white;
    text-align: center;
    position: fixed;
    top: 0;
    right: 0;
    width: 100vw;
    padding: 10px 0px;
    font-weight: bold;
    z-index: -1;
}
</style>