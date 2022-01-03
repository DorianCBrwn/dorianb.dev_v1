<script>
	export let name = '';
	export let viewBox = extractViewBox(name);

	export let size = '20px';
	export let width = size;
	export let height = size;
	export let color = 'currentColor';
	export let stroke = color;
	export let fill = color;
	// Todo: custome script and add animation support
	$: elements = name.replace(/<svg ([^>]*)>/, '').replace('</svg>', '');

	function extractViewBox(svg) {
		const regex = /viewBox="([\d- ]+)"/;
		const res = regex.exec(svg);
		if (!res) return '0 0 20 20'; // default value
		return res[1];
	}
</script>

<svg xmlns="http://www.w3.org/2000/svg" {width} {height} {viewBox} {stroke} {fill} {...$$restProps}>
	{@html elements}
</svg>
<svg xmlns="http://www.w3.org/2000/svg" width="55" height="55" fill="none" viewBox="0 0 55 55">
	<g class="Icon2">
		<path
			stroke="#FEFCFB"
			stroke-width="2"
			d="M28 4c14.36 0 26 11.64 26 26S42.36 56 28 56l-8.5 8V44.5l-8 14.5h-8"
			class="outer-d-path"
		/>
		<path fill="#FEFCFB" d="M30 46c8.837 0 16-7.163 16-16s-7.163-16-16-16v32z" class="inner-d" />
		<circle cx="25" cy="4" r="3.5" stroke="#FEFCFB" class="head-circle" />
		<circle cx="2" cy="59" r="1.5" stroke="#FEFCFB" class="tail-circle" />
		<circle cx="12" cy="65" r="1" fill="#FEFCFB" class="small-circle" />
		<circle cx="27" cy="74" r="2" fill="#FEFCFB" class="large-cirlce" />
		<circle cx="35" cy="62" r="2" fill="#FEFCFB" class="medium-circle" />
	</g>
</svg>
