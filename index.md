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
				'00DWL000002dfgT',
				'eCommerce_Messaging',
				'https://healthstream--hstm.sandbox.my.site.com/ESWeCommerceMessaging1754589994624',
				{
					scrt2URL: 'https://healthstream--hstm.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://healthstream--hstm.sandbox.my.site.com/ESWeCommerceMessaging1754589994624/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
