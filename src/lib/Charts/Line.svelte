<script>
	import { Line } from 'svelte-chartjs';
	import { data3 } from '../Charts_Data/data';

	import {
		Chart as ChartJS,
		Title,
		Tooltip,
		Legend,
		LineElement,
		LinearScale,
		PointElement,
		CategoryScale
	} from 'chart.js';

	ChartJS.register(Title, Tooltip, Legend, LineElement, LinearScale, PointElement, CategoryScale);
</script>

<Line data={data3} options={{ responsive: true }} />
