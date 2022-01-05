<script setup>
import Card from "./layout/Card.vue";
import Progress from "./layout/Progress.vue";
import Exp from "./layout/Exp.vue";
import Projects from "./layout/Projects.vue";
import Blog from "./layout/Blog.vue";
import Hobby from "./layout/Hobby.vue";
import Footer from "./layout/Footer.vue";
</script>

<template>
	<section class="mt-10 mb-1 space-y-10 sm:space-y-5 lg:mx-40">
		<Card />
		<div class="lg:flex lg:justify-between lg:items-center">
			<Progress />
		<Exp />
		</div>
		<Projects />
		<div class="sm:flex sm:items-start">
			<Blog />
			<Hobby />
		</div>
		<Footer />
	</section>
</template>
