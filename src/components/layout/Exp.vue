<script setup>
import { ref } from "vue";
import mehran from "../../assets/images/mh-pack-1.png";
import fasirous from "../../assets/images/fasirous-leather.png";

const experience = ref([
	{
		src: mehran,
		date: "مهر ۹۱ - فروردین ۹۳",
		title: "عضو تیم شرکت تیم مهران پک",
		description:
			"مهران پک مجرب در زمینه طراحی ، چاپ و تولید انواع جعبه های فانتزی",
	},
	{
		src: fasirous,
		date: "خرداد ۹۳ - اردیبهشت ۹۷",
		title: "سرپرست تیم در توسعه طراحی",
		description:
			"شرکت فاسیروس پیشرو در بازار تهران در صنعت اکسسوری‌های چرمی اصیل",
	},
	{
		src: mehran,
		date: "فروردین ۹۷ - اسفند ۱۴۰۰",
		title: "عضو تیم شرکت چاپ ",
		description:
			"شرکت فاسیروس پیشرو در بازار تهران در صنعت اکسسوری‌های چرمی اصیل",
	},
]);
</script>

<template>
	<section class="p-5 m-5 bg-white rounded-md">
		<h1 class="text-xl font-bold tracking-wide">تجارب</h1>
		<div class="exp">
			<div v-for="exp in experience" :key="exp" class="">
				<div class="flex items-center space-y-7">
					<img :src="exp.src" alt="company logo" class="w-24 pl-5 mb-7" />
					<div>
						<h4 class="pb-1 text-xs tracking-tighter sub-text">
							{{ exp.date }}
						</h4>
						<h1 class="text-xs font-bold">{{ exp.title }}</h1>
						<p class="pt-3 text-xs sub-text">
							{{ exp.description }}
						</p>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>

<style scoped>
.exp:last-child{
  margin-bottom: .5rem;
}
</style>
