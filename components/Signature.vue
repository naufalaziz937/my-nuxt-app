<template>
    <section class="bg-gray-100 py-20">
        <div class="max-w-6xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-10 px-4">
            <div>
                <h3 class="text-2xl font-semibold mb-2">Signature blend.</h3>
                <p class="text-sm text-gray-600 max-w-md mb-10">
                    Rhoncus massa, turpis, volutpat ut erat magna erat, mauris aenean mauris vitae. Donec malesuada sollicitudin sodales pulvinar nec. Nulla vehicula dolor nunc, sed consectetur.
                </p>
            </div>
            <div class="relative">
                <div class="flex space-x-6 overflow-x-auto pb-4 hide-scrollbar snap-x snap-mandatory">
                    <Card
                        img="/images/kemasan.png"
                        title="themoon"
                        subtitle="Lunar Roast"
                        rating="★★★★★"
                    />
                    <Card
                        img="/images/kemasan.png"
                        title="thesun"
                        subtitle="Citrus Weather"
                        rating="★★★★☆"
                    />
                    <Card
                        img="/images/kemasan.png"
                        title="therain"
                        subtitle="Caramel Haze"
                        rating="★★★★★"
                    />
                    <Card
                        img="/images/kemasan.png"
                        title="thewind"
                        subtitle="Cold Breeze"
                        rating="★★★★★"
                    />
                </div>
                <div class="absolute left-0 right-0 bottom-0 flex justify-center mt-2 pointer-events-none">
                    <div class="w-16 h-1 bg-gray-300 rounded-full relative">
                        <div class="w-1/3 h-1 bg-black rounded-full animate-scroll-indicator"></div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import Card from '@/components/Card.vue'

export default {
    components: {
        Card
    }
}
</script>

<style scoped>
.hide-scrollbar::-webkit-scrollbar {
    display: none;
}
.hide-scrollbar {
    -ms-overflow-style: none;
    scrollbar-width: none;
}
@keyframes scroll-indicator {
    0% {
        margin-left: 0;
    }
    100% {
        margin-left: 66%;
    }
}
.animate-scroll-indicator {
    animation: scroll-indicator 2s infinite alternate;
}
</style>