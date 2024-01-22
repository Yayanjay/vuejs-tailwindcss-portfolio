<script>
import feather from 'feather-icons';

export default {
    name: 'Home',
    data: () => {
        return {
            theme: '',
        };
    },
    created() {
        this.theme = localStorage.getItem('theme') || 'light';
    },
    mounted() {
        feather.replace();
        this.theme = localStorage.getItem('theme') || 'light';
    },
    updated() {
        feather.replace();
    },
    methods: {},
};
</script>

<template>
    <main class="grid min-h-full place-items-center bg-white dark:bg-primary-dark py-24 px-6 sm:py-32 lg:px-8">
		<div class="text-center ">
			<p class="text-base font-general-bold text-indigo-600">404</p>
				<h1 class="mt-4 text-3xl font-general-semibold tracking-tight text-ternary-dark dark:text-ternary-light sm:text-5xl">Page not found</h1>
			<p class="mt-6 font-general-regular leading-7 text-ternary-dark dark:text-ternary-light">Sorry, we couldn’t find the page you’re looking for.</p>
			<div class="mt-10 flex items-center justify-center gap-x-6">
				<a href="/" class="rounded-md bg-indigo-600 px-3.5 py-2.5 text-sm font-general-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Go back home</a>
			</div>
		</div>
    </main>
</template>

<style lang="scss" scoped></style>