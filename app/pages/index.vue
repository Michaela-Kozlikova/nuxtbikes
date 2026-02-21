<script setup>
const bikes = [
							{ id: 1, name: 'Honda CBR', img: '/pics/moto-gallery/honda-cbr-repsol.jpg'},
							{ id: 2, name: 'Honda CBR 1000RR', img: '/pics/moto-gallery/honda-CBR1000rr.jpeg'},
							{ id: 3, name: 'Honda Hornet', img: '/pics/moto-gallery/honda-hornet.jpg'},
							{ id: 4, name: 'Honda XL 750 Transalp', img: '/pics/moto-gallery/honda-xl750-transalp.jpeg'},
							{ id: 5, name: 'Honda Rebel', img: '/pics/moto-gallery/honda-rebel.jpeg'},
							{ id: 6, name: 'Suzuki Hayabusa', img: '/pics/moto-gallery/suzuki-hayabusa.jpg'},
							{ id: 7, name: 'Suzuki Intruder', img: '/pics/moto-gallery/suzuki-intruder.jpg'},
							{ id: 8, name: 'Suzuki V-Strom', img: '/pics/moto-gallery/suzuki-v-strom.jpeg'},
							{ id: 9, name: 'Suzuki SV 650', img: '/pics/moto-gallery/suzuki-sv650.jpg'},
							{ id: 10, name: 'Suzuki GSX-S', img: '/pics/moto-gallery/suzuki-gsx-s.jpg'},
							{ id: 11, name: 'Kawasaki Z900', img: '/pics/moto-gallery/kawasaki-z900.jpg'},
							{ id: 12, name: 'Kawasaki Versys-X 300', img: '/pics/moto-gallery/kawasaki-versys-x300.jpeg'},
							{ id: 13, name: 'Kawasaki Vulcan-S', img: '/pics/moto-gallery/kawasaki-vulcan-s.jpg'},
							{ id: 14, name: 'Kawasaki KX', img: '/pics/moto-gallery/kawasaki-kx.jpg'},
							{ id: 15, name: 'Kawasaki H2R', img: '/pics/moto-gallery/kawasaki-h2r.jpg'},
							{ id: 16, name: 'Yamaha MT-09', img: '/pics/moto-gallery/yamaha-mt-09.jpg'},
							{ id: 17, name: 'Yamaha XSR', img: '/pics/moto-gallery/yamaha-xsr.jpg'},
							{ id: 18, name: 'Yamaha XVS Dragstar', img: '/pics/moto-gallery/yamaha-xvs-dragstar.jpg'},
							{ id: 19, name: 'Yamaha R1', img: '/pics/moto-gallery/yamaha-r1.jpg'},
							{ id: 20, name: 'Yamaha Ténéré', img: '/pics/moto-gallery/yamaha-tenere.jpg'}
						]
</script>

<template>
      <div class="main-content">
          <h2 class="article-title">Proč právě japonské motorky?</h2>
          <div class="article-image">
            <img src= "/pics/logo.jpeg" alt="Superbike logo" width="350" height="300" loading="lazy" decoding="async" />
            <p> Japonské značky si vydobyly pověst díky dokonalému spojení výkonu, spolehlivosti a moderní technologie. Od prvních modelů až po dnešní legendy udávají směr a určují, jak má vypadat skutečná silniční motorka. Jsou navržené tak, aby zvládly jak svižnou jízdu městem, tak dlouhé výlety po otevřených silnicích. Precizní zpracování a smysl pro detail z nich dělají stroje, které vydrží a neztratí své kouzlo ani po letech. Ať už hledáš čistý výkon, nadčasový design, nebo spolehlivého parťáka na každodenní cesty, v japonských motorkách najdeš všechno dohromady. </p>
          </div>
          <h2 class="article-title">Poznej legendy</h2>
          <div class="article-image">
            <img src= "/pics/speed_indicator.jpg" alt="Speed indicator" width="350" height="300" />
            <p> Od Hondy přes Yamahu až po Suzuki a Kawasaki – značky, které určují směr světa silničních motorek. Každá z nich má svůj vlastní příběh, jedinečný styl. Jsou to stroje, které si získaly srdce jezdců po celém světě. <br /> Vyber si svou oblíbenou značku a objev modely, které se staly legendami dvou kol. </p>
          </div>
          <h2 class="article-title">O mně</h2>
			<p>Holka, co má ráda rychlý motorky a stylový auta, ale vlastní jen řidičák sk. B &#128516. Ráda cestuju (hlavně letadlem), ochutnávám alkohol a steaky. Chci se naučit španělsky a japonsky, dělat hezký webovky a mít se fajn &#10084.
			<br>
			Dost o mně, teď jdeme mrknout na moje nejoblíbenější <strong>modely</strong>.</p>
        <div class="video-section">
          <div class="video-wrapper">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/54rvxXP65P8?si=9fRxBrDluFU5MY6h&amp;controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen loading="lazy"></iframe>
          </div>
        </div>
				<h2>Další japonské skvosty</h2>
				<div class="gallery-grid">
					<BikeCard
			v-for="bike in bikes"
			:key="bike.id"
			:name="bike.name"
			:image="bike.img"/>
				</div>
        <div class="faq-section">
          <h3>Nejčastější dotazy</h3>
          <details>
            <summary> Jaká je maximální rychlost Hondy CBR? <svg class="arrow-icon lucide lucide-chevron-down" xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M6 9l6 6 6-6" /> </svg>
            </summary>
            <p>Honda CBR může dosahovat rychlosti až 299 km/h, záleží na modelu a úpravách.</p>
          </details>
          <details>
            <summary> Který model Suzuki je nejlepší pro začátečníky? <svg class="arrow-icon lucide lucide-chevron-down" xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M6 9l6 6 6-6" /> </svg>
            </summary>
            <p>Pro začátečníky se doporučuje Suzuki GSX-S 750 nebo V-Strom 650 díky vyvážené hmotnosti a ovladatelnosti.</p>
          </details>
          <details>
            <summary> Jak často je potřeba servisovat Kawasaki Ninja? <svg class="arrow-icon lucide lucide-chevron-down" xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M6 9l6 6 6-6" /> </svg>
            </summary>
            <p>Servis závisí na modelu a používání, ale doporučuje se každých 6000–8000 km nebo 12 měsíců.</p>
          </details>
        </div>
				<div class="pages-visit-counter js-pages-visit-counter">
          <table>
            <thead>
              <tr>
                <th>Počet návštěv</th>
								<th> </th>
              </tr>
            </thead>
            <tbody>
							<tr>
								<td style="color: rgb(20, 170, 20);">Online</td>
								<td class="js-online-count">0</td>
							</tr>
              <tr>
                <td>Týdně</td>
								<td class="js-weekly-count">0</td>
              </tr>
              <tr>
                <td>Měsíčně</td>
								<td class="js-monthly-count">0</td>
              </tr>
              <tr>
                <td><b>Celkem</b></td>
								<td class="js-total-count">0</td>
              </tr>
            </tbody>
          </table>
         </div>
        </div>
</template>

<style scoped>

.main-content {
	display: flex;
	flex-direction: column;
	padding: 60px;
}

.article-image {
	display: flex;
	gap: 20px;
	align-items: center;
	margin-bottom: 100px;
	flex-direction: row;
	justify-content: left;
}

.article-image p {
	max-width: 400px;
	text-align: start;
}

img {
	border-radius: 10px;
}

.video-section {
	display: flex;
	justify-content: center;
	padding: 80px;
}

.video-wrapper {
	width: 100%;
	max-width: 900px;
	aspect-ratio: 16 / 9;
}

.video-wrapper iframe {
	width: 100%;
	height: 100%;
	border: 0;
}

.gallery-grid {
	display: grid;
	justify-items: center;
	gap: 1rem;
	max-width: 1200px;
	margin: 0 auto;
	grid-template-columns: repeat(5, 1fr);
}

.faq-section {
	max-width: 660px;
   	color: white;
	padding-top: 100px;
}

h3 {
	color: yellow;
}

details {
	border-bottom: solid 0.5px yellow;
}

summary {
	display: flex;
	align-items: center;
	justify-content: space-between;
	font-weight: bold;
	margin: -0.5rem -0.5rem 0;
	padding: 1rem;
	cursor: pointer;
	list-style: none;
}

details[open] summary {
	margin-bottom: 0.5rem;
}

details[open] p {
	padding-left: 6px;
}

.arrow-icon {
	transition: transform 0.3s ease;
	color: yellow;
}

details[open] .arrow-icon {
	transform: rotate(180deg);
}

.pages-visit-counter {
	display: flex;
	justify-content: center;
	padding-top: 100px;
}

table {
	color: rgb(7, 7, 7);
	border: 1px solid black;
	border-collapse: collapse;
	width: 140px;
}

thead {
	background-color: #23a8d1;
}

tbody {
	background-color: rgb(235, 235, 235);
}
</style>