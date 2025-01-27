<html>
  <body>
    <script type='text/javascript'>
	  function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			        window.addEventListener("onEmbeddedMessagingReady", () => {
            embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({
                "PreChat_URL": window.location.origin
            });
        });
 
			embeddedservice_bootstrap.init(
				'00D300000006Vym',
				'Streamy_ShiftWizard',
				'https://healthstream.my.site.com/ESWStreamyShiftWizard1737139032082',
				{
					scrt2URL: 'https://healthstream.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://healthstream.my.site.com/ESWStreamyShiftWizard1737139032082/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
  </body>
</html>
