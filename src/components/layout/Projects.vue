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
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import "swiper/css/pagination";
import SwiperCore, { Autoplay, Pagination, Navigation } from "swiper";

// install Swiper modules
SwiperCore.use([Autoplay, Pagination, Navigation]);

const projects = ref([
	{
		mobile: covidMobile,
		desktop: covidDesktop,
		t1: "vuejs#",
		t2: "tailwind#",
		t3: "html#",
		title: "ردیاب کووید",
		desctription:
			"پروژه‌ <strong>ردیاب کووید</strong> این فرصت رو به من داد تا تجربه	بیشتری در کار با <strong>API</strong> و<strong>Asynchronous</strong> در جاوااسکریپت کسب کنم.",
		live: "https://kind-mccarthy-32f3f6.netlify.app/",
		code: "https://github.com/Dellcash/covid-tracker",
	},
	{
		mobile: vawMobile,
		desktop: vawDesktop,
		t1: "vuejs#",
		t2: "bootstrap#",
		t3: "css#",
		title: "ووآو",
		desctription:
			"در این پروژه من به مفهوم <strong>resuable component</strong> در <strong>vuejs</strong> پی بردم و به راحتی به سادگی به کار بردم.",
		live: "https://vaw.netlify.app/blog",
		code: "https://github.com/Dellcash/Single-page-application",
	},
	{
		mobile: whicoMobile,
		desktop: whicoDesktop,
		t1: "vuejs#",
		t2: "quasar#",
		t3: "firebase#",
		title: "ویکوو",
		desctription:
			"<strong>ویکوو</strong> یک پروژه <strong>fullstack</strong> هست که با استفاده از  <strong>vuejs</strong> و <strong>firebase</strong> پیاده سازی شده و وب اپلیکشن محسوب می‌شود.",
		live: "https://whico.netlify.app/",
		code: "https://github.com/Dellcash/whico",
	},
	{
		mobile: tomedoMobile,
		desktop: tomedoDesktop,
		t1: "vuejs#",
		t2: "vuetify#",
		t3: "html#",
		title: "تومیدوو",
		desctription:
			"در این پروژه من با استفاده از <strong>localstorage</strong> تونستم بکار بگیرم و به راحتی اطلاعات کاربر رو در مرورگر ذخیره کنم.",
		live: "https://to-me-do.netlify.app/#/",
		code: "https://github.com/Dellcash/to-me-do",
	},
	{
		mobile: urlShortenerMobile,
		desktop: urlShortenerDesktop,
		t1: "petitevue#",
		t2: "tailwind#",
		t3: "responsive#",
		title: "آدرس کوتاه",
		desctription:
			"این پروژه <strong>frontend mentor challenge</strong> است. در این پروژه <strong>rel.ink API</strong> برای ایجاد <strong>URL</strong> کوتاه شده و نمایش آنها مطابق طرح داده شده است.",
		live: "https://infallible-ardinghelli-cc223b.netlify.app/",
		code: "https://github.com/Dellcash/URL-shortening",
	},
]);
</script>

<template>
	<section>
		<div class="px-5 py-2 mx-5 mb-3 bg-white rounded-lg lg:mt-6">
			<h1 class="text-xl font-bold tracking-wide lg:text-2xl">پروژه‌ها (۵)</h1>
		</div>
		<swiper
			:spaceBetween="30"
			:centeredSlides="true"
			:autoplay="{
				delay: 2500,
				disableOnInteraction: false,
			}"
			:pagination="{
				clickable: true,
			}"
			:navigation="true"
			class="mySwiper"
		>
			<swiper-slide
				v-for="project in projects"
				:key="project"
				class="mb-10"
			>
				<div class="p-5 mx-5 bg-white rounded-lg">
					<!-- project images -->
					<div class="flex w-full p-4 mb-4 bg-blue-100 rounded-lg md:p-8">
						<img
							:src="project.mobile"
							alt="mobile view"
							class="w-10 rounded-lg md:w-24 mobile"
						/>
						<img
							:src="project.desktop"
							alt="desktop view"
							class="pr-2 desktop md:pr-6"
						/>
					</div>
					<!-- details -->
					<div>
						<div class="flex text-sm text-blue-500 lg:text-lg tag">
							<h4 class="pl-3">{{ project.t3 }}</h4>
							<h4 class="pl-3">{{ project.t2 }}</h4>
							<h4>{{ project.t1 }}</h4>
						</div>
						<div class="mt-4">
							<h1 class="pb-2 text-lg font-bold lg:text-2xl title">
								{{ project.title }}
							</h1>
							<p
								class="text-sm tracking-tighter sub-text lg:text-lg lg:w-3/5 desc"
								v-html="project.desctription"
							></p>
						</div>
						<div class="mt-8 text-sm btn">
							<button
								class="
									ml-2
									rounded-lg
									bg-blue-500
									text-white
									py-1.5
									px-4
									tracking-tighter
									shadow-md
									hover:bg-white hover:text-blue-500 hover:border-blue-500
								"
							>
								<a :href="project.live" target="_blank">پیش‌نمایش</a>
							</button>
							<button
								class="px-8 py-1 text-blue-500 border-2 border-blue-500 rounded-lg shadow-md hover:bg-blue-500 hover:text-white hover:border-transparent"
							>
								<a :href="project.code" target="_blank">کد</a>
							</button>
						</div>
					</div>
				</div>
			</swiper-slide>
		</swiper>
	</section>
</template>

<style scoped>
.sp {
	width: 88.5% !important;
}
@media (max-width: 320px) {
	.sp {
		width: 87.2% !important;
	}
	.desktop {
		width: 10.5rem;
	}
}
@media (min-width: 375px) {
	.desktop {
		width: 13.6rem;
	}
}
@media (min-width: 425px) {
	.sp {
		width: 90.7% !important;
	}
	.desktop {
		width: 15.9rem;
	}
	.mobile {
		width: 3.4rem;
	}
}
@media (min-width: 640px) {
	.sp {
		width: 94.8% !important;
	}
	.desktop {
		width: 31.7rem;
	}
	.mobile {
		width: 7.4rem;
	}
}

@media (min-width: 1024px) {
	.sp {
		width: 96% !important;
	}
	.desktop {
		width: 44.4rem;
	}
	.mobile {
		width: 11rem;
	}
}

@media (min-width: 1440px) {
	.sp {
		width: 96.5% !important;
	}
	.desktop {
		width: 49rem;
	}
	.mobile {
		width: 12rem;
	}
	.tag {
		font-size: 1.3rem;
	}
	.title {
		font-size: 1.8rem;
	}
	.desc {
		font-size: 1.3rem;
		padding-top: 0.5rem;
		width: 70%;
	}
	.btn {
		font-size: 1.3rem;
	}
	.btn button:first-child {
		padding: 1rem 2rem;
	}
	.btn button:last-child {
		padding: 15px 3.5rem;
	}
}
</style>
