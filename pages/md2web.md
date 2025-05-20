## Outline template
	- [[Logseq Site Demo V2]]
	  title:: My Enhanced Logseq Site
	  lang:: en
		- ## Main Navigation
		  section_type:: header
		  logo_text:: MySiteLogo
	- # Nav links are children of the header block
		- Home
		  element_type:: link
		  link_url:: #hero-section
		- Features
		  element_type:: link
		  link_url:: #features
		- Projects
		  element_type:: link
		  link_url:: #our-projects
		- About
		  element_type:: link
		  link_url:: #about-us
		- Contact
		  element_type:: link
		  link_url:: #contact
		- ## Welcome to Our Dynamic Site!
		  id:: hero-section
		  section_type:: hero
		  image_src:: /placeholder-hero-abstract.jpg
		  image_alt:: Colorful abstract waves background
	- # Hero content elements are children of the hero section block
		- #hero_title Next-Gen Web Experiences
		  element_type:: title
		- Transform your Logseq notes into stunning, interactive websites. Explore the future of content.
		  element_type:: paragraph
		- Explore Features
		  element_type:: button
		  link_url:: #features
		- ## Core Features
		  id:: features
		  section_type:: list_block
		  section_title:: What We Offer
	- # List items are children
		- **Intuitive Logseq Parsing:** Seamlessly convert outlines to structured HTML.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- **Tailwind CSS Styling:** Modern, responsive designs built-in.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- **Flexible Section Types:** Headers, heroes, content, lists, projects, and footers.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- **Customizable Layouts:** Content blocks with image-left, image-right, or single-column.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- ## Our Projects
		  id:: our-projects
		  section_type:: projects
		  section_title:: Discover Our Work
	- # Project items are children of this block
		- Project Innovate
		  element_type:: project_item # Optional, can be inferred if direct child of 'projects'
		  project_title:: Project Innovate # Overrides main content if present
		  project_thumbnail_src:: /placeholder-project-tech.jpg
		  project_thumbnail_alt:: Tech project abstract visual
		  project_description:: A groundbreaking platform using AI to enhance productivity and streamline workflows for creative teams.
		  project_link_url:: #
		  project_link_text:: View Case Study
		- EcoScapes Initiative
		  element_type:: project_item
		  project_title:: EcoScapes Initiative
		  project_thumbnail_src:: /placeholder-project-nature.jpg
		  project_thumbnail_alt:: Nature-inspired project visual
		  project_description:: Developing sustainable solutions for urban green spaces, promoting biodiversity and community well-being.
		  project_link_url:: #
		  project_link_text:: Explore EcoScapes
		- Artfolio Connect
		  element_type:: project_item
		  project_title:: Artfolio Connect
		  project_thumbnail_src:: /placeholder-project-art.jpg
		  project_thumbnail_alt:: Artistic project visual
		  project_description:: A digital gallery and networking hub for emerging artists to showcase their work and connect with collectors.
		  project_link_url:: #
	- # project_link_text defaults to "View Project"
		- QuantumLeap Analytics
		  element_type:: project_item
		  project_title:: QuantumLeap Analytics
		  project_thumbnail_src:: /placeholder-project-data.jpg
		  project_thumbnail_alt:: Data analytics project visual
		  project_description:: Advanced data analytics tool providing deep insights for businesses to make informed decisions.
		  project_link_url:: #
		- Culinary Adventures App
		  element_type:: project_item
		  project_title:: Culinary Adventures App
		  project_thumbnail_src:: /placeholder-project-food.jpg
		  project_thumbnail_alt:: Food related project visual
		  project_description:: An interactive mobile app for food lovers to discover new recipes, restaurants, and culinary events.
		  project_link_url:: #
		- SpaceVoyager VR
		  element_type:: project_item
		  project_title:: SpaceVoyager VR
		  project_thumbnail_src:: /placeholder-project-space.jpg
		  project_thumbnail_alt:: Space exploration project visual
		  project_description:: A virtual reality experience that takes users on an immersive journey through our solar system and beyond.
		  project_link_url:: #
		- ## About Our Journey
		  id:: about-us
		  section_type:: content_block
		  layout:: image_left
		  section_title:: The Story Behind Our Innovation
	- # Columns are children
		- Image Column
		  column:: image
			- ![Team discussing ideas](/placeholder-team-dynamic.jpg)
			  element_type:: image
			  image_alt:: Diverse team brainstorming with enthusiasm
		- Text Column
		  column:: content
			- ### From Notes to Narratives
			  element_type:: title
			- We started with a simple idea: empower Logseq users to share their knowledge beautifully. Our journey is about bridging thought organization with compelling web presentation.
			  element_type:: paragraph
			- We support [[Open Source]] principles and believe in [[Community Collaboration]]. This tool is for [[Content Creators]] and [[Knowledge Workers]].
			  element_type:: paragraph
		- ## Why Partner With Us?
		  section_type:: content_block
	- # No layout property implies default single column, centered text.
	  section_title:: The Advantages
	- # Content elements are direct children
		- ### Effortless Creation
		  element_type:: title
		- Transform complex Logseq outlines into structured HTML with minimal effort.
		  element_type:: paragraph
		- ### Blazing Speed
		  element_type:: title
		- Generate previews instantly and download your complete static site in seconds.
		  element_type:: paragraph
		  class:: italic text-center # Custom class example
		- ### Cutting-Edge Design
		  element_type:: title
		- Utilizes Tailwind CSS for a professional, responsive, and modern aesthetic.
		  element_type:: paragraph
		- ## Get In Touch
		  id:: contact
		  section_type:: content_block
		  section_title:: We're Here to Help
	- # Content elements are direct children
		- ### Reach Out
		  element_type:: title
		- For inquiries, support, or feedback, connect with us.
		  element_type:: paragraph
		- Email Our Team
		  element_type:: button
		  link_url:: mailto:support@example.com
		  class:: mt-4
		- ## Site Footer
		  section_type:: footer
		  id:: page-footer
	- # Footer content items are children
		- ©  MySiteName. All rights reserved. | [[Privacy Policy]] | [[Terms of Service]]
		  element_type:: paragraph
- ## Sample outline
	- [[Alma Flamenca - Web Oficial]] # Este es el bloque raíz de la página (Nivel 0)
	  title:: Alma Flamenca - La Fusión del Duende
	  lang:: es
	- # Este bloque no necesita section_type ni ID, es solo el contenedor lógico.
		- ## Encabezado del Sitio # Bloque de Nivel 1 - Sección Header
		  section_type:: header
	- # ID sanitizado será "encabezado-del-sitio". No requiere id:: explícito.
	  logo_text:: Alma Flamenca
	- # Los enlaces de navegación pueden ser hijos con element_type:: link
		- Inicio
		  element_type:: link
		  link_url:: #la-esencia-de-alma-flamenca # Enlace a una sección por su ID
		- Música
		  element_type:: link
		  link_url:: #discografia
		- Gira
		  element_type:: link
		  link_url:: #proximos-eventos
		- Contacto
		  element_type:: link
		  link_url:: #contacta-con-alma
		- ## La Esencia de Alma Flamenca # Bloque de Nivel 1 - Sección Hero
		  section_type:: hero
	- # ID sanitizado será "la-esencia-de-alma-flamenca"
	  image_src:: img/alma-hero.webp # Imagen principal del héroe
	  image_alt:: Alma Flamenca en vivo, escenario vibrante
		- #hero_title Alma Flamenca # Este tag ayuda al parser a identificar el tipo de elemento
		  element_type:: title # H2 inferido del ##
	- # Aquí el parser debería aplicar clases de título grandes y estilos de Hero
		- El Flamenco que rompe fronteras con sonidos innovadores.
		  element_type:: paragraph # Párrafo base, que el script estilizará como subtítulo de Hero
	- # Aquí el parser debería aplicar clases de subtítulo de Hero
		- Escucha su último single
		  element_type:: button
		  link_url:: https://open.spotify.com/artist/almaflamencaXYZ # URL del botón de acción
		  link_target:: _blank
	- # Aquí el parser debería aplicar clases de botón
		- ## Sobre Alma Flamenca # Bloque de Nivel 1 - Sección de Contenido con Imagen
		  section_type:: content_block
	- # ID sanitizado será "sobre-alma-flamenca"
	  layout:: image_left # Define el layout: imagen a la izquierda, contenido a la derecha
		- Columna de Imagen # Bloque hijo para agrupar la imagen
		  column:: image # Define que este bloque y sus hijos van en la columna de imagen
			- ![Alma Flamenca - Retrato](img/alma-bio.webp) # Puedes usar sintaxis Markdown o property
	- # O con propiedad explícita:
	- #
	  element_type:: image
	- #
	  image_src:: img/alma-bio.webp
	- #
	  image_alt:: Retrato del cantaor
		- Columna de Texto # Bloque hijo para agrupar el contenido de texto
		  column:: content # Define que este bloque y sus hijos van en la columna de contenido
			- ### Una Voz que Transciende
			  element_type:: title # H3 inferido del ###. Se aplica a este bloque.
			- Nacido en el corazón de Andalucía, Alma Flamenca fusiona la pasión ancestral con ritmos electrónicos y sonoridades globales.
			  element_type:: paragraph # Párrafo normal. Se aplica a este bloque.
			- Su música explora nuevas texturas manteniendo siempre la pureza del cante jondo. Ha colaborado con artistas de diversos géneros, llevando el flamenco a nuevos públicos.
			  element_type:: paragraph
		- ## Discografía Reciente # Bloque de Nivel 1 - Sección de Lista Simple
		  section_type:: list_block
		  id:: discografia # Usamos propiedad id:: porque el encabezado es diferente
		  section_title:: Álbumes y Singles Destacados # Título central para la sección
		- Álbum "Caminos Nuevos" (2024): Explorando fusiones inéditas.
		  element_type:: list_item # Este bloque es un ítem de lista
		  highlight_first_sentence:: true # Pone "Álbum 'Caminos Nuevos' (2024)" en negrita
		- Single "Ritmo del Mar" (2024): Sonido fresco y bailable.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- EP "Raíces Urbanas" (2023): Homenaje al flamenco de barrio.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- ## Próximos Eventos
		  section_type:: list_block # Otra sección de lista
	- # ID sanitizado será "proximos-eventos". Notar que "Música" usó "discografia" y no "discografia-reciente", evitando un duplicado directo basado en el encabezado, pero si hubieran coincidido, se añadiría el sufijo.
	  section_title:: Gira 2025
		- 18 Mayo - Teatro Central, Sevilla: Entradas agotadas.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- 25 Mayo - Palau de la Música, Barcelona: Últimas entradas disponibles.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- 7 Junio - Live House, Londres, UK: ¡Primera vez en la ciudad!
		  element_type:: list_item
		  highlight_first_sentence:: true
		- ## Contacta con Alma
		  section_type:: content_block # Sección simple para contacto
		  id:: contacta-con-alma # Usamos propiedad id:: para un ID más específico
		- ### Booking y Prensa
		  element_type:: title # H3
		- Para consultas profesionales, entrevistas o contrataciones, por favor contacte a través del siguiente email.
		  element_type:: paragraph
		- Enviar Email a Alma
		  element_type:: button
		  link_url:: mailto:management@almaflamenca.com
		  link_target:: _blank
		- ## Información Legal
		  section_type:: footer # Tipo de sección para el pie de página
		  id:: pie-de-pagina # ID explícito
		- © 2025 Alma Flamenca. Todos los derechos reservados. | Aviso Legal | Política de Privacidad
		  element_type:: paragraph # Contenido del footer
	- # Aquí podrías tener sub-bloques para los enlaces legales si quieres que sean clicleables