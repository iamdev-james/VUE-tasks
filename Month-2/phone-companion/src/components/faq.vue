<template>
	<div class="w-2/3">
		<div class="text-center mb-16">
			<p class="text-blue-dark font-semibold">FREQUENT QUESTIONS</p>
			<p class="text-3xl font-bold">Do you have any question</p>
		</div>
		<div>
			<div class="mb-6">
				<div class="relative mb-12">
					<img v-show="box_1" :src="require('@/assets/images/open.svg')" class="absolute" />
					<img v-show="!box_1" :src="require('@/assets/images/close.svg')" class="absolute" />
					<p class="ml-12">How to contact with riders emergency ?</p>
				</div>
				<span
					><p class="ml-12">
						Get your website ads tests delivered at let collect sample from the
						victory of the managements that supplies best design system which
						guidelines ever with multiple features.
					</p></span
				>
			</div>
      <hr>
			<div class="mb-6">
				<div class="relative mb-12">
					<img v-show="box_2" :src="require('@/assets/images/open.svg')" class="absolute" />
					<img v-show="!box_2" :src="require('@/assets/images/close.svg')" class="absolute" />
					<p class="ml-12">How to contact with riders emergency ?</p>
				</div>
				<span
					><p class="ml-12">
						Get your website ads tests delivered at let collect sample from the
						victory of the managements that supplies best design system which
						guidelines ever with multiple features.
					</p></span
				>
			</div>
      <hr>
			<div class="mb-6">
				<div class="relative mb-12">
					<img v-show="box_3" :src="require('@/assets/images/open.svg')" class="absolute" />
					<img v-show="!box_3" :src="require('@/assets/images/close.svg')" class="absolute" />
					<p class="ml-12">How to contact with riders emergency ?</p>
				</div>
				<span
					><p class="ml-12">
						Get your website ads tests delivered at let collect sample from the
						victory of the managements that supplies best design system which
						guidelines ever with multiple features.
					</p></span
				>
			</div>
      <hr>
			<div class="mb-6">
				<div class="relative mb-12">
					<img v-show="box_4" :src="require('@/assets/images/open.svg')" class="absolute" />
					<img v-show="!box_4" :src="require('@/assets/images/close.svg')" class="absolute" />
					<p class="ml-12">How to contact with riders emergency ?</p>
				</div>
				<span
					><p class="ml-12">
						Get your website ads tests delivered at let collect sample from the
						victory of the managements that supplies best design system which
						guidelines ever with multiple features.
					</p></span
				>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: "faq-comp",
    data() {
      return {
        box_1: false,
        box_2: false,
        box_3: false,
        box_4: true
      }
    },
	}
</script>
