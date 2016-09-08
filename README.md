# Browser-tab-opener
Automatically opens browsers and tabs


package broswerOpener;
import java.awt.Desktop;
import java.io.IOException;
import java.net.URI;
import java.net.URISyntaxException;

public class Main {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		
	    //Checks if the Computer can run the "desktop method", doesnt work on Apple devices and some distros of Linux
		if(Desktop.isDesktopSupported())
		{
		  try {
			Desktop.getDesktop().browse(new URI("http://sc10pfinesses01.blackbaud.global/desktop/container/?locale=en_US"));
			Desktop.getDesktop().browse(new URI("http://10.10.9.46/cwfo/apps/Schedule.html?userLang=en&userTheme=calabrio&userCountry=#/scheduling/agentSchedules"));
			Desktop.getDesktop().browse(new URI("http://fiveguys/managers/ctdpro.aspx?user="));
			Desktop.getDesktop().browse(new URI("http://bbkb.blackbaud.com/#f:@articlefilters:not=[Archived]&f:@articlefilters:operator=or"));
		} catch (IOException e) {
			// TODO Auto-generated catch block
			e.printStackTrace();
		} catch (URISyntaxException e) {
			// TODO Auto-generated catch block
			e.printStackTrace();
		}
		}
	}

}
