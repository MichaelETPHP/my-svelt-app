
<script context="module">
	export async function load({ fetch }) {
		const res = await fetch('https://jsonplaceholder.typicode.com/posts');
		const users = await res.json();
		// console.log(users);
		if (res.ok) {
			return {
				props: {
					users
				}
			};
		}

		return {
			status: res.status,
			error: new Error('Could not fetch the Users')
		};
	}
</script>
<script>
	export let users;
</script>



  <!-- ======= Hero Section ======= -->
  <section id="hero" class="">
    <div class="container" data-aos="zoom-in" data-aos-delay="100">
      <h1>Brandon Johnson</h1>
      
      <p>I'm <span class="typed" data-typed-items="Designer, Developer, Freelancer, Photographer"></span></p>
      <div class="social-links">
        <a href="#" class="twitter"><i class="bx bxl-twitter"></i></a>
        <a href="#" class="facebook"><i class="bx bxl-facebook"></i></a>
        <a href="#" class="instagram"><i class="bx bxl-instagram"></i></a>
        <a href="#" class="google-plus"><i class="bx bxl-skype"></i></a>
        <a href="#" class="linkedin"><i class="bx bxl-linkedin"></i></a>
      </div>
    </div>
  </section><!-- End Hero -->
  <main id="main">
      <!-- ======= About Section ======= -->
      <section id="about" class="about">
        <div class="container" data-aos="fade-up">
          <div class="section-title">
            <h2>About</h2>
            <p>
              Magnam dolores commodi suscipit. Necessitatibus eius consequatur
              ex aliquid fuga eum quidem. Sit sint consectetur velit. Quisquam
              quos quisquam cupiditate. Et nemo qui impedit suscipit alias ea.
              Quia fugiat sit in iste officiis commodi quidem hic quas.
            </p>
          </div>

          <div class="row">
            <div class="col-lg-4">
              <img src="assets/img/profile-img.jpg" class="img-fluid" alt="" />
            </div>
            <div class="col-lg-8 pt-4 pt-lg-0 content">
              <h3>UI/UX Designer &amp; Web Developer.</h3>
              <p class="fst-italic">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.
              </p>
              <div class="row">
                <div class="col-lg-6">
                  <ul>
                    <li>
                      <i class="bi bi-chevron-right"></i>
                      <strong>Birthday:</strong> <span>1 May 1995</span>
                    </li>
                    <li>
                      <i class="bi bi-chevron-right"></i>
                      <strong>Website:</strong> <span>www.example.com</span>
                    </li>
                    <li>
                      <i class="bi bi-chevron-right"></i>
                      <strong>Phone:</strong> <span>+123 456 7890</span>
                    </li>
                    <li>
                      <i class="bi bi-chevron-right"></i>
                      <strong>City:</strong> <span>New York, USA</span>
                    </li>
                  </ul>
                </div>
                <div class="col-lg-6">
                  <ul>
                    <li>
                      <i class="bi bi-chevron-right"></i> <strong>Age:</strong>
                      <span>30</span>
                    </li>
                    <li>
                      <i class="bi bi-chevron-right"></i>
                      <strong>Degree:</strong> <span>Master</span>
                    </li>
                    <li>
                      <i class="bi bi-chevron-right"></i>
                      <strong>PhEmailone:</strong>
                      <span>email@example.com</span>
                    </li>
                    <li>
                      <i class="bi bi-chevron-right"></i>
                      <strong>Freelance:</strong> <span>Available</span>
                    </li>
                  </ul>
                </div>
              </div>
              <p>
                Officiis eligendi itaque labore et dolorum mollitia officiis
                optio vero. Quisquam sunt adipisci omnis et ut. Nulla
                accusantium dolor incidunt officia tempore. Et eius omnis.
                Cupiditate ut dicta maxime officiis quidem quia. Sed et
                consectetur qui quia repellendus itaque neque. Aliquid amet
                quidem ut quaerat cupiditate. Ab et eum qui repellendus omnis
                culpa magni laudantium dolores.
              </p>
            </div>
          </div>
        </div>
      </section>
      <!-- End About Section -->
      </main>
      

         <!-- ======= Resume Section ======= -->
      <section id="resume" class="resume">
        <div class="container" data-aos="fade-up">
          <div class="section-title">
            <h2>Resume</h2>
            <p>
              Magnam dolores commodi suscipit. Necessitatibus eius consequatur
              ex aliquid fuga eum quidem. Sit sint consectetur velit. Quisquam
              quos quisquam cupiditate. Et nemo qui impedit suscipit alias ea.
              Quia fugiat sit in iste officiis commodi quidem hic quas.
            </p>
          </div>

          <div class="row">
            <div class="col-lg-6">
              <h3 class="resume-title">Sumary</h3>
              <div class="resume-item pb-0">
                <h4>Brandon Johnson</h4>
                <p>
                  <em
                    >Innovative and deadline-driven Graphic Designer with 3+
                    years of experience designing and developing user-centered
                    digital/print marketing material from initial concept to
                    final, polished deliverable.</em
                  >
                </p>
                <ul>
                  <li>Portland par 127,Orlando, FL</li>
                  <li>(123) 456-7891</li>
                  <li>alice.barkley@example.com</li>
                </ul>
              </div>

              <h3 class="resume-title">Education</h3>
              <div class="resume-item">
                <h4>Master of Fine Arts &amp; Graphic Design</h4>
                <h5>2015 - 2016</h5>
                <p><em>Rochester Institute of Technology, Rochester, NY</em></p>
                <p>
                  Qui deserunt veniam. Et sed aliquam labore tempore sed
                  quisquam iusto autem sit. Ea vero voluptatum qui ut
                  dignissimos deleniti nerada porti sand markend
                </p>
              </div>
              <div class="resume-item">
                <h4>Bachelor of Fine Arts &amp; Graphic Design</h4>
                <h5>2010 - 2014</h5>
                <p><em>Rochester Institute of Technology, Rochester, NY</em></p>
                <p>
                  Quia nobis sequi est occaecati aut. Repudiandae et iusto quae
                  reiciendis et quis Eius vel ratione eius unde vitae rerum
                  voluptates asperiores voluptatem Earum molestiae consequatur
                  neque etlon sader mart dila
                </p>
              </div>
            </div>
            <div class="col-lg-6">
              <h3 class="resume-title">Professional Experience</h3>
              <div class="resume-item">
                <h4>Senior graphic design specialist</h4>
                <h5>2019 - Present</h5>
                <p><em>Experion, New York, NY </em></p>
                <ul>
                  <li>
                    Lead in the design, development, and implementation of the
                    graphic, layout, and production communication materials
                  </li>
                  <li>
                    Delegate tasks to the 7 members of the design team and
                    provide counsel on all aspects of the project.
                  </li>
                  <li>
                    Supervise the assessment of all graphic materials in order
                    to ensure quality and accuracy of the design
                  </li>
                  <li>
                    Oversee the efficient use of production project budgets
                    ranging from $2,000 - $25,000
                  </li>
                </ul>
              </div>
              <div class="resume-item">
                <h4>Graphic design specialist</h4>
                <h5>2017 - 2018</h5>
                <p><em>Stepping Stone Advertising, New York, NY</em></p>
                <ul>
                  <li>
                    Developed numerous marketing programs (logos,
                    brochures,infographics, presentations, and advertisements).
                  </li>
                  <li>
                    Managed up to 5 projects or tasks at a given time while
                    under pressure
                  </li>
                  <li>
                    Recommended and consulted with clients on the most
                    appropriate graphic design
                  </li>
                  <li>
                    Created 4+ design presentations and proposals a month for
                    clients and account managers
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- End Resume Section -->




  
<!-- <center><h1>List off Post</h1></center>
{#each users as user}
	<a sveltekit:prefetch href={`/singleuser/${user.id}`}>{user.title}</a>
	<hr />
{/each} -->


