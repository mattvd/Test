Test
====

			<div class="application-content">
				<?php
				if( is_user_logged_in() ) { ?>
			<?php
				/**
				 * job_manager_application_details_email or job_manager_application_details_url hook
				 */
				do_action( 'job_manager_application_details_' . $apply->type, $apply );
			?>
			<?php } else 
				echo 'Hey there.  You have to register for free <a href="/register">here</a> to be able to see this listing. It&#39;s for <b>free</b>, promise!';
			}
			?>
