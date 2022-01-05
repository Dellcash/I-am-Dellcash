<script setup>
import { ref } from "vue";
import guitar from "../../assets/images/guitar.png";
import leather from "../../assets/images/leather.png";
import walking from "../../assets/images/walk.png";

const hobbies = ref([
	{
		src: guitar,
		alt: "نواختن گیتار",
		title: "ساز زدن",
		description: "تقریبا ۱/۳ عمرم با نواختن گیتار گذروندم.",
	},
	{
		src: leather,
		alt: "کار با چرم",
		title: "کار با چرم",
		description: "علاقه‌مندیم به کار با چرم از هنرهای دستی نشأت گرفته.",
	},
	{
		src: walking,
		alt: "پیاده‌روی",
		title: "پیاده روی",
		description:
			"پیاده‌روی این امکان بم میده تا ذهنم رو خالی کنم و باعث میشه ایده‌های جالبی برای خودم بگیرم.",
	},
]);
</script>

<template>
	<section class="p-5 m-5 bg-white rounded-lg">
		<h1 class="text-lg font-bold tracking-wide lg:text-xl">تفریحات</h1>
		<div class="mt-5 space-y-5 hobby">
			<div class="text-sm lg:text-lg" v-for="hobby in hobbies" :key="hobby">
				<img
					:src="hobby.src"
					:alt="hobby.alt"
					class="object-cover w-full h-24 rounded-md md:h-32 "
				/>
				<h1 class="font-bold mt-3.5 pr-1">{{ hobby.title }}</h1>
				<p class="pt-2.5 pr-1 tracking-tight sub-text lg:text-sm">{{ hobby.description }}</p>
			</div>
		</div>
	</section>
</template>

<style scoped>
@media (min-width: 1440px){
	.hobby div{
		padding-bottom: 14px
	}
}
</style>