<html>
   <body>
	<script type='text/javascript'>
		function initEmbeddedMessaging() {
			try {
				embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

    				/* START:: Conversation Opened Listener */
				window.addEventListener( "onEmbeddedMessagingConversationOpened", ( event ) => {
				
					console.log( "START:: Conversation Opened" );
					console.log( "Event detail: ", JSON.stringify( event.detail ) );
     					console.log( "Page location is " + window.location.href );
					console.log( "END:: Conversation Opened" );
				
				} );
    				/* END:: Conversation Opened Listener */
    
				embeddedservice_bootstrap.settings.chatButtonPosition = "50px,50px";
				embeddedservice_bootstrap.init(
					'00Dau000002ItPt',
					'MIAW',
					'https://infallibletechiemiaworg.my.site.com/ESWMIAW1720544291552',
					{
						scrt2URL: 'https://infallibletechiemiaworg.my.salesforce-scrt.com'
					}
				);
			} catch (err) {
				console.error('Error loading Embedded Messaging: ', err);
			}
		};
	</script>
	<script type='text/javascript' src='https://infallibletechiemiaworg.my.site.com/ESWMIAW1720544291552/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
   </body>
</html>
