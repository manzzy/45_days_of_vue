<template>
    <section class="testimonials">
        <div class="content">
            <div class="testimonials-header">
                <span class="section-indicator">Testimonials</span>
                <h2>What Our customers <br> Say about us</h2>
            </div>

            <ul class="testimonial-list">
                <li class="testimonial-card" v-for="testimonial in testimonials" :key="testimonial.author.name">
                    <p class="testimonial-text">
                        "{{ testimonial.text }}"
                    </p>
                    <div class="testimonial-author">
                        <img :src="testimonial.author.img_link" :alt="testimonial.author.img_alt" />
                        <div class="author-info">
                            <span class="author-name">{{ testimonial.author.name }}</span>
                            <span class="author-role">{{ testimonial.author.role }}</span>
                        </div>
                    </div>
                </li>

            </ul>
        </div>
    </section>
</template>

<script setup> 
    const testimonials = [
        {
            text: "The team at DentalCare is amazing! They made me feel so comfortable during my root canal treatment. Highly recommend!",
            author: {
                name: "Sarah M.",
                role: "Patient",
                img_link: "https://randomuser.me/api/portraits/women/8.jpg",
                img_alt: "User Photo: Sarah M."
            }
        },
        {
            text: "I had a fantastic experience at DentalCare. The staff were friendly and professional, the procedure was quick and painless, and my smile has never looked better. Highly recommend!",
            author: {
                name: "John D.",
                role: "Patient",
                img_link: "https://randomuser.me/api/portraits/men/78.jpg",
                img_alt: "User Photo: John D."
            }
        },
        {
            text: "As a mom, I felt completely at ease bringing my child to DentalCare. The staff were warm and patient, explained every step, and made the visit stress-free. My child left smiling — we couldn't be happier!",
            author: {
                name: "Fatima M.",
                role: "Mother",
                img_link: "https://randomuser.me/api/portraits/women/68.jpg",
                img_alt: "User Photo: Fatima M."
            }
        },
        {
            text: "At 52, I was nervous about visiting the dentist again, but the team treated me like family. They were patient, gentle, and explained everything. I left with a warm smile and a lighter heart — I couldn't be happier!",
            author: {
                name: "Alex W.",
                role: "Patient",
                img_link: "https://randomuser.me/api/portraits/men/22.jpg",
                img_alt: "User Photo: Alex W."
            }
        }
    ]
</script>

<style scoped>
    @import url('../assets/styles/testimonials.css');
</style>