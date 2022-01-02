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
	<section class="p-5 m-5 bg-white rounded-lg sm:flex">
		<img
			src="../../assets/images/dellcash.png"
			alt="photo of me"
			class="rounded-lg sm:w-48"
		/>
		<div class="pt-3 space-y-3 sm:pr-5 sm:pt-0">
			<div class="space-y-3 sm:flex sm:items-center sm:pb-2 sm:justify-between">
				<div>
					<h1 class="text-2xl font-bold tracking-tight">امید دلکش</h1>
					<h4 class="sub-text">فرانت‌_اند دولوپر</h4>
				</div>
				<div class="info">
					<div v-for="inf in info" :key="inf">
						<h4 class="flex items-end sub-text">
							<span class="pl-2 text-xl material-icons">{{ inf.icon }}</span
							><a
								:href="inf.href"
								target="_blank"
								class="tracking-tight sm:tracking-tighter hover:text-black"
								>{{ inf.title }}</a
							>
						</h4>
					</div>
				</div>
			</div>
			<div
				class="tracking-wide sm:tracking-tight text-sm sm:space-y-2 sub-text"
			>
				<p class="w-5/6">
					<!-- من <strong>جونیور</strong> دولوپر هستم. <br> -->
					توسعه دهنده <strong>خود‌آموخته</strong> و با <strong>انگیزه</strong>،
					که مایل به <strong>یادگیری</strong> و ایجاد برنامه های کاربردی
					<strong>UI برجسته</strong> است.
				</p>
				<p class="hidden sm:block w-4/6">
					من روی نوشتن <strong>HTML قابل دسترس</strong> ، استفاده از
					<strong>شیوه های مدرن CSS</strong> و نوشتن
					<strong>جاوا اسکریپت تمیز</strong> تمرکز می کنم.
				</p>
			</div>
		</div>
	</section>
</template>

<style scoped>
.info div:last-child h4 a {
	letter-spacing: 0.5px;
}
</style>
