<template>
  <footer>
  	<dl>
  		<dt>Email</dt>
  		<dd><a :href="stero">rexsteroxy22@gmail.com</a></dd>
  	</dl>
  	<dl>
  		<dt>Phone</dt>
  		<dd><a :href="tel">+2349037096290</a></dd>
  	</dl>
  	<dl class="mb-0">
  		<dt>Find me on</dt>
  		<dd class="mb-0">
  			<ul class="nav nav-social">
  				<li class="nav-item">
  					<a class="nav-link" href="https://www.facebook.com/amadiaustin.77" target="_blank">
  						<i class="fa fa-facebook"></i>
  					</a>
  				</li>
  				<li class="nav-item">
  					<a class="nav-link" href="https://www.linkedin.com/in/amadiaustinchukwuemeka/" target="_blank">
  						<i class="fa fa-linkedin"></i>
  					</a>
  				</li>
  				<li class="nav-item">
  					<a class="nav-link" href="https://twitter.com/AMADIAUSTINCHU1" target="_blank">
  						<i class="fa fa-twitter"></i>
  					</a>
  				</li>
  				<li class="nav-item">
  					<a class="nav-link" href="https://github.com/rexsteroxy" target="_blank">
  						<i class="fa fa-github"></i>
  					</a>
  				</li>
  			</ul>
  		</dd>
  	</dl>
  </footer>
</template>

<script>
export default {
	data(){
		return {
			email: 'rexsteroxy22@gmail.com',
			phone: '+234 90 37 09 62 90',
			social : {
				facebook : '',
				twitter: '',
				github: ''
			}
		}
	},
	computed: {
		stero(){
			return 'stero:' + this.email;
		},
		tel(){
			return 'tel:' + this.phone.replace(/ /g, '')
		}
	}
}
</script>
