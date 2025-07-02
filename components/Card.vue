    <template>
    <div
        class="min-w-[200px] bg-black px-20 py-12 text-white rounded-md text-center flex-shrink-0 snap-center shadow-lg hover:scale-105 transition-transform duration-300"
    >
        <img :src="img" alt="themoon" class="w-20 mx-auto mb-4" />
        <p class="font-medium text-sm">{{ title }}</p>
        <p class="text-xs text-gray-400">{{ subtitle }}</p>
        <p class="text-yellow-400 mt-1 text-sm">{{ rating }}</p>
    </div>
    </template>

    <script>
    export default {
    props: {
        img: { type: String, required: true },
        title: { type: String, required: true },
        subtitle: { type: String, required: true },
        rating: { type: String, required: true },
    },
    };
    </script>
