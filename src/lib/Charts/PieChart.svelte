<script>
	import { Pie } from 'svelte-chartjs';
	import { data2 } from '../Charts_Data/data';

	import { Chart as ChartJS, Title, Tooltip, Legend, ArcElement, CategoryScale } from 'chart.js';

	ChartJS.register(Title, Tooltip, Legend, ArcElement, CategoryScale);
</script>

<Pie data={data2} options={{ responsive: true }} />
