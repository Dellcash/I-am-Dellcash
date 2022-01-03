<script setup>
import { ref } from "vue";
import mehran from "../../assets/images/mh-pack-1.png";
import fasirous from "../../assets/images/fasirous-leather.png";
import sepano from "../../assets/images/sepano.png";

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
		title: "سرپرست تیم توسعه و طراحی فاسیروس",
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
	<section class="p-5 m-5 bg-white rounded-lg lg:w-3/6 lg:mt-0 lg:mr-0">
		<h1 class="text-xl font-bold tracking-wide">تجارب</h1>
		<div class="exp sm:flex lg:block">
			<div v-for="exp in experience" :key="exp" class="sm:w-1/3 lg:w-full">
				<div
					class="flex items-center space-y-7 sm:space-y-0 sm:items-start sm:mt-4 lg:space-y-7"
				>
					<a :href="exp.href" target="_blank" class="w-60 sm:w-48 lg:w-32 lg:mt-8"
						><img
							:src="exp.src"
							alt="company logo"
							class="pl-5 mb-7 sm:pl-2 sm:mb-10 lg:pl-3"
					/></a>
					<div class="text-xs lg:text-sm">
						<h4 class="pb-1 tracking-tighter sub-text">
							{{ exp.date }}
						</h4>
						<h1 class="font-bold tracking-tighter">{{ exp.title }}</h1>
						<p class="pt-3 sub-text lg:w-5/6">
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
</style>
