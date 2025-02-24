<script lang="ts">
	import {
		MapLibre,
		Marker,
		NavigationControl,
		ScaleControl,
		GlobeControl
	} from 'svelte-maplibre-gl';
</script>

<MapLibre
	class="h-[55vh] min-h-[300px]"
	style="https://basemaps.cartocdn.com/gl/voyager-gl-style/style.json"
	zoom={3.5}
	center={{ lng: 137, lat: 36 }}
>
	<NavigationControl />
	<ScaleControl />
	<GlobeControl />

	<Marker lnglat={[141.350714, 43.068564]} />
</MapLibre>
