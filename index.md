<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			window.addEventListener("onEmbeddedMessagingReady", () => {
				embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({
					"PreChat_URL": "https://www.cme.com/test"
				});
			});

			embeddedservice_bootstrap.init(
				'00DWL000003W4Bd',
				'Messaging_eCommerce',
				'https://healthstream--hstm.sandbox.my.site.com/ESWMessagingeCommerce1761573851220',
				{
					scrt2URL: 'https://healthstream--hstm.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://healthstream--hstm.sandbox.my.site.com/ESWMessagingeCommerce1761573851220/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
