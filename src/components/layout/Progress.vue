<template>
	<div class="">
		<section dir="ltr" class="p-5 m-5 bg-white rounded-lg md:mt-0 front">
			<h1 style="direction: rtl" class="mb-3 text-xl font-bold">فرانت_اند</h1>
			<div
				class="space-y-2 tracking-tighter md:flex md:items-start md:space-y-0 md:space-x-10 lg:block lg:space-x-0 lg:space-y-3"
			>
				<div class="space-y-2 md:w-1/2 lg:w-full lg:space-y-3">
					<!-- Vue -->
					<div class="flex items-center justify-between space-x-5">
						<h3>Vue</h3>
						<div
							class="
								w-full
								bg-gray-200
								rounded-full
								h-2.5
								dark:bg-gray-700
								w-3/4
							"
						>
							<div
								class="bg-blue-600 h-2.5 rounded-full"
								style="width: 55%"
							></div>
						</div>
					</div>
					<!-- Tailwind -->
					<div class="flex items-center justify-between space-x-5">
						<h3 class="tailwind">Tailwind</h3>
						<div
							class="
								w-full
								bg-gray-200
								rounded-full
								h-2.5
								dark:bg-gray-700
								w-3/4
							"
						>
							<div
								class="bg-blue-600 h-2.5 rounded-full"
								style="width: 65%"
							></div>
						</div>
					</div>
					<!-- Css -->
					<div class="flex items-center justify-between space-x-5">
						<h3>Css</h3>
						<div
							class="
								w-full
								bg-gray-200
								rounded-full
								h-2.5
								dark:bg-gray-700
								w-3/4
							"
						>
							<div
								class="bg-blue-600 h-2.5 rounded-full"
								style="width: 65%"
							></div>
						</div>
					</div>
				</div>
				<div class="space-y-2 md:w-1/2 lg:w-full lg:space-y-3">
					<!-- Nuxt -->
					<div class="flex items-center justify-between space-x-5">
						<h3>Nuxt</h3>
						<div
							class="
								w-full
								bg-gray-200
								rounded-full
								h-2.5
								dark:bg-gray-700
								w-3/4
							"
						>
							<div
								class="bg-blue-600 h-2.5 rounded-full"
								style="width: 45%"
							></div>
						</div>
					</div>
					<!-- Pinia -->
					<div class="flex items-center justify-between space-x-5">
						<h3>Pinia</h3>
						<div
							class="
								w-full
								bg-gray-200
								rounded-full
								h-2.5
								dark:bg-gray-700
								w-3/4
							"
						>
							<div
								class="bg-blue-600 h-2.5 rounded-full"
								style="width: 35%"
							></div>
						</div>
					</div>
				</div>
			</div>
		</section>
		<section
			dir="ltr"
			class="hidden p-5 m-5 bg-white rounded-lg design lg:block md:mt-0 md:w-1/3 lg:mt-6"
		>
			<h1 style="direction: rtl" class="mb-3 text-xl font-bold">طراحی</h1>
			<div class="space-y-2 tracking-tighter lg:space-y-3">
				<!-- Figma -->
				<div class="flex items-center justify-between space-x-5">
					<h3 class="pr-5">Figma</h3>
					<div class="w-full bg-gray-200 rounded-full h-2.5 dark:bg-gray-700">
						<div
							class="bg-blue-600 h-2.5 rounded-full"
							style="width: 35%"
						></div>
					</div>
				</div>
				<!-- Photoshop -->
				<div class="flex items-center space-x-3">
					<h3>Photoshop</h3>
					<div class="w-full bg-gray-200 rounded-full h-2.5 dark:bg-gray-700">
						<div
							class="bg-blue-600 h-2.5 rounded-full"
							style="width: 15%"
						></div>
					</div>
				</div>
			</div>
		</section>
	</div>
</template>

<style scoped>
@media (min-width: 320px){
	.tailwind{
		margin-right: -1rem;
	}
}
@media (min-width: 1024px) {
	.front {
		width: 28rem;
	}
	.design {
		width: 28rem;
	}
}
</style>
