<script setup>
import { ref } from "vue";
import mehran from "../../assets/images/mh-pack-1.png";
import fasirous from "../../assets/images/fasirous-leather.png";
import sepano from '../../assets/images/sepano.png'

const experience = ref([
	{
		src: mehran,
		href: "https://mehranpack.com/",
		date: "مهر ۹۱ - فروردین ۹۳",
		title: "عضو تیم شرکت مهران پک",
		description:
			"مهران پک مجرب در زمینه طراحی ، چاپ و تولید انواع جعبه های فانتزی",
	},
	{
		src: fasirous,
		href: "tel:+989109201292",
		date: "خرداد ۹۳ - اردیبهشت ۹۷",
		title: "سرپرست تیم توسعه و طراحی",
		description:
			"شرکت فاسیروس پیشرو در بازار تهران در صنعت اکسسوری‌های چرمی اصیل",
	},
	{
		src: sepano,
		href: "tel:+989122904930",
		date: "فروردین ۹۷ - اسفند ۱۴۰۰",
		title: "عضو تیم شرکت چاپ سپانو",
		description:
			"شرکت سپانو مستقر در جلوب تهران که ارائه کننده خدمات چاپ و طراحی پوشاک است.",
	},
]);
</script>

<template>
	<section class="p-5 m-5 bg-white rounded-lg lg:w-1/2 lg:mt-0 lg:mr-0">
		<h1 class="text-xl font-bold tracking-wide lg:pb-0.5">تجارب</h1>
		<div class="exp md:flex lg:block">
			<div v-for="exp in experience" :key="exp" class="md:w-1/3 lg:w-full">
				<div class="flex items-center space-y-7 md:space-y-0 md:items-start md:mt-4">
					<a :href="exp.href" target="_blank" class="w-60 md:w-48 lg:w-28"
						><img :src="exp.src" alt="company logo" class="pl-5 mb-7 md:pl-2 md:mb-10"
					/></a>
					<div class="text-xs lg:text-sm">
						<h4 class="pb-1 tracking-tighter sub-text">
							{{ exp.date }}
						</h4>
						<h1 class="font-bold tracking-tighter">{{ exp.title }}</h1>
						<p class="pt-3 sub-text lg:w-4/5">
							{{ exp.description }}
						</p>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>

<style scoped>
.exp:last-child {
	margin-bottom: 0.5rem;
}
@media (min-width: 768px) {
	.exp div:last-child div a img {
		width: 6.5rem;
		max-width: none;
	}
}
</style>
