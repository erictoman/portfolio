<script>
	let certifications = [
		{
			issuer: 'Checkmarx',
			date: '2021-08-01',
			name: 'Checkmarx Certified Engineer'
		},
		{
			name: 'Accessible Website Design',
			description: 'Specialized in designing accessible websites for a user-friendly experience.'
		},
		{
			name: 'Java Data Handling with Hibernate',
			description: 'Utilized Hibernate, a Java framework, for effective data handling.'
		},
		{
			name: 'Image Analysis Techniques',
			description: 'Acquired expertise in analyzing and interpreting images.'
		},
		{
			name: 'Build Web Apps with React JS',
			description: 'Developed web applications from scratch using React JS.'
		},
		{
			name: 'Mobile App Development with React Native',
			description: 'Created mobile applications using React Native.'
		},
		{
			name: 'Java Web Development with Spring',
			description: 'Implemented web development using the Spring framework for Java.'
		},
		{
			name: 'Web Services Development (Java)',
			description: 'Focused on creating and consuming web services in Java.'
		}
	];
</script>

<section>
	<article>
		<h2>Courses and certifications</h2>
		<ul class="courses-list">
			{#each certifications as certification}
				<li>
					{certification.issuer ? `${certification.issuer} - ` : ''}
					{certification.date
						? new Date(certification.date).toLocaleDateString('en-US', {
								year: 'numeric',
								month: 'long',
								day: 'numeric'
							})
						: ''}
					{certification.name}
					{certification.description ? ` - ${certification.description}` : ''}
				</li>
			{/each}
		</ul>
		<p>
			If you are interested in my certificates, you can find them in my <a
				href="https://github.com/erictoman/cursos">Github</a
			> repository.
		</p>
	</article>
</section>
