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
	<section class="space-y-10 mb-1 mt-10 sm:space-y-5">
		<Card />
		<Progress />
		<Exp />
		<Projects />
		<div class="sm:flex sm:items-start">
			<Blog />
			<Hobby />
		</div>
		<Footer />
	</section>
</template>
