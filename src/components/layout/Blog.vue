<script setup>
import { ref } from "vue";
import blog_1 from "../../assets/images/blog-1.png";

const blogs = ref([
	{
		title: "وضعیت ویوو در ۲۰۲۱",
		src: blog_1,
		subTitle:
			'<strong>"One Piece"</strong> نام نسخه سوم ویو‌جی‌اس است. "آپدیت‌های بزرگویوو هر کدوم با یه اسم انیمه خاص نام‌گذاری می‌شن."',
		description:
			'		ويژگی‌های مهمی که به این نسخه اضافه شد می‌شه اشاره کرد به <br /><strong>"Composition API" </strong><br /><strong>"Teleport"</strong><br /><strong>"Fragments"</strong><br /><strong>"v-modelهای بیشتر"</strong><br /><strong>"سرعت"</strong><br />و ...',
	},
]);
</script>

<template>
	<section>
		<div
			class="
				relative
				z-10
				p-5
				m-5
				md:ml-0
				overflow-x-hidden
				bg-white
				rounded-lg
			"
			v-for="blog in blogs"
			:key="blog"
		>
			<div class="flex mt-2">
				<div class="tracking-wide w-28">
					<h4 class="mb-5 text-xs opacity-50">وبلاگ‌</h4>
					<h1 class="text-xl font-bold leading-6">{{ blog.title }}</h1>
				</div>
				<div class="img">
					<img :src="blog.src" alt="blog picture" />
				</div>
			</div>
			<div class="text-md mt-60 md:mt-64 md:pt-2.5 desc">
				<p class="sub-text" v-html="blog.subTitle"></p>
				<br />
				<p class="hidden md:block sub-text" v-html="blog.description"></p>
				<h1 class="font-bold text-blue-500 lg:pt-3 md:text-left">
					<a href="https://vaw.netlify.app/">بیشتر...</a>
				</h1>
			</div>
		</div>
	</section>
</template>

<style scoped>
strong {
	color: #4f4f4f;
}
.img {
	width: 100%;
	position: absolute;
	right: 5rem;
	z-index: -1;
}

@media (max-width: 320px) {
		.desc{
		margin-top: 13rem;
	}
}

@media (min-width: 375px){
	.desc{
		margin-top: 17rem;
	}
}

@media (min-width: 425px) {
	.desc{
		margin-top: 20rem;
	}
}

@media (min-width: 640px) {
	.img {
		right: 8rem;
		width: 87%;
	}

	.desc {
		margin-top: 18rem;
	}
}
</style>
