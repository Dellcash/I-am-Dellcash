<template>
	<section class="relative z-10 p-5 m-5 sm:ml-0 overflow-x-hidden bg-white rounded-lg">
		<div class="flex mt-2">
			<div class="tracking-wide w-28">
				<h4 class="mb-5 text-xs opacity-50">وبلاگ‌</h4>
				<h1 class="text-xl font-bold leading-6">وضعیت ویوو در ۲۰۲۱</h1>
			</div>
			<div class="img">
				<img src="../../assets/images/blog-1.png" alt=""/>
			</div>
		</div>
		<div class="text-sm mt-60 sm:mt-64 sm:pt-2.5">
			<p class="sub-text">
				<strong>"One Piece"</strong> نام نسخه سوم ویو‌جی‌اس است. "آپدیت‌های بزرگ
				ویوو هر کدوم با یه اسم انیمه خاص نام‌گذاری می‌شن."
			</p>
			<br />
			<p class="hidden sm:block">
				ويژگی‌های مهمی که به این نسخه اضافه شد می‌شه اشاره کرد به <br /><strong
					>"Composition API" </strong
				><br /><strong>"Teleport"</strong><br /><strong>"Fragments"</strong
				><br /><strong>"v-modelهای بیشتر"</strong><br /><strong>"سرعت"</strong
				><br />و ...
			</p>
			<h1 class="font-bold text-blue-500 lg:pt-3">
				<a href="https://vaw.netlify.app/">بیشتر...</a>
			</h1>
		</div>
	</section>
</template>

<style scoped>
.img {
	width: 100%;
	position: absolute;
	right: 5rem;
	z-index: -1;
}

@media (min-width: 640px) {
	.img {
		right: 7rem;
		width: 90%;
	}
}
</style>
