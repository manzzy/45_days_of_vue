<template>
    <section class="ratings">
        <div class="content">
            <ul class="ratings-list">
                <li class="rating-item" v-for="rating in ratings" :key="rating.tag">
                    <span class="tag">{{ rating.tag }}</span>
                    <span class="rating-num">{{ rating.ratingNum }}</span>
                    <span class="rating-txt" v-html="rating.ratingTxt.replace(/\n/g, '<br />')"></span>
                </li>

            </ul>
        </div>
    </section>
</template>

<script setup> 
    const ratings = [
        {
            tag: 'For All time we grow',
            ratingNum: '98%',
            ratingTxt: 'All Time patient \nsatisfaction rate'
        },
        {
            tag: 'For current 3 years',
            ratingNum: '4.9/5',
            ratingTxt: 'Star Rating on \nGoogle Reviews'
        },
        {
            tag: 'For current 5 years',
            ratingNum: '10K+',
            ratingTxt: 'Happy Patients and \nStill Growing'
        },
        {
            tag: 'For every dentist',
            ratingNum: '20+',
            ratingTxt: 'Years of Experience in \nDental Excellence'
        }
    ]
</script>

<style scoped>
    @import url('../assets/styles/ratings.css');
</style>