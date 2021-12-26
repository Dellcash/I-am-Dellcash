<script setup>
import { ref } from "vue";

const info = ref([
	{
		icon: "mail",
		title: "omiddellcash@gmail.com",
		href: "mailto: omiddellcash@gmail.com",
	},
	{
		icon: "phone",
		title: "۰۹۳۵۳۴۱۷۳۵۲",
		href: "tel:+989353417352",
	},
]);
</script>

<template>
	<section class="p-5 m-5 bg-white rounded-md">
		<img src="../../assets/images/dellcash.png" alt="photo of me" class="rounded-md" />
		<div class="pt-3 space-y-3">
			<div>
				<h1 class="text-2xl font-bold tracking-tight">امید دلکش</h1>
				<h4 class="sub-text">فرانت‌_اند دولوپر</h4>
			</div>
			<div class="info">
				<div v-for="inf in info" :key="inf">
					<h4 class="flex items-end">
						<span class="pl-2 text-xl material-icons">{{ inf.icon }}</span
						><a
							:href="inf.href"
							target="_blank"
							class="tracking-tight hover:text-black"
							>{{ inf.title }}</a
						>
					</h4>
				</div>
			</div>
			<div class="text-sm sub-text">
				<p class="w-4/5 tracking-wide">
					توسعه دهنده <strong>خود‌آموخته</strong> و با <strong>انگیزه</strong>،
					که مایل به <strong>یادگیری</strong> و ایجاد برنامه های کاربردی
					<strong>UI برجسته</strong> است.
				</p>
			</div>
		</div>
	</section>
</template>

<style scoped>
/* .info div:last-child h4 a {
	letter-spacing: .5px;
} */
</style>
