<script setup>
import { ref } from "vue";
import covidMobile from "../../assets/images/covid-mobile.png";
import covidDesktop from "../../assets/images/covid.png";
import vawMobile from "../../assets/images/vaw-mobile.png";
import vawDesktop from "../../assets/images/vaw.png";
import whicoMobile from "../../assets/images/whico-mobile.png";
import whicoDesktop from "../../assets/images/whico.png";
import tomedoMobile from "../../assets/images/tomedo-mobile.png";
import tomedoDesktop from "../../assets/images/tomedo.png";
import urlShortenerMobile from "../../assets/images/url-shortener-mobile.png";
import urlShortenerDesktop from "../../assets/images/url-shortener.png";

const projects = ref([
	{
		mobile: covidMobile,
		desktop: covidDesktop,
	},
	{
		mobile: vawMobile,
		desktop: vawDesktop,
	},
	{
		mobile: whicoMobile,
		desktop: whicoDesktop,
	},
	{
		mobile: tomedoMobile,
		desktop: tomedoDesktop,
	},
	{
		mobile: urlShortenerMobile,
		desktop: urlShortenerDesktop,
	},
]);
</script>

<template>
	<section>
		<div class="px-5 py-2 mx-5 mb-3 bg-white rounded-md">
			<h1 class="text-xl font-bold tracking-wide">پروژه‌ها</h1>
		</div>
		<div class="space-y-5">
			<div v-for="project in projects" :key="project" class="p-5 mx-5 bg-white rounded-md">
      <!-- project images -->
				<div class="flex w-full p-4 mb-4 bg-blue-100 rounded-md">
					<img
						:src="project.mobile"
						alt="mobile view"
						class="w-10 rounded-md"
					/>
					<img :src="project.desktop" alt="desktop view" class="w-48 pr-2" />
				</div>
        <!-- details -->
				<div>
				<div class="flex text-xs">
					<h4 class="pl-3">HTML#</h4>
					<h4 class="pl-3">TAILWINDCSS#</h4>
					<h4>VUEJS#</h4>
				</div>
				<div class="mt-4">
					<h1 class="pb-2 text-lg font-bold">ردیاب کوید</h1>
					<p class="text-sm tracking-tight">
						پروژه‌ <strong>ردیاب کوید</strong> این فرصت رو به من داد تا تجربه
						بیشتری کار با <strong>API</strong> و
						<strong>Asynchronous</strong> در جاوااسکریپت کسب کنم.
					</p>
				</div>
				<div class="mt-8 text-sm">
					<button
						class="
							ml-2
							rounded-md
							bg-blue-500
							text-white
							py-1.5
							px-4
							tracking-tighter
							hover:bg-white hover:text-blue-500 hover:border-blue-500
						"
					>
						<a href="">پیش‌نمایش</a>
					</button>
					<button
						class="px-8 py-1 text-blue-500 border-2 border-blue-500 rounded-md hover:bg-blue-500 hover:text-white hover:border-transparent"
					>
						<a href="">کد</a>
					</button>
				</div>
			</div>
			</div>
		</div>
	</section>
</template>
