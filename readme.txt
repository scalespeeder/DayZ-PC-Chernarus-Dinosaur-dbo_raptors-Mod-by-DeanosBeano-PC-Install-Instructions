DayZ Chernarus PC Dinosaur / Raptor dbo_raptors Mod by DeanosBeano PC Install Instructions & Terms Of Use

Many thanks to DeanosBeano for creating this amazing mod. Please visit his Discord and if you can,
contribute to his projects: https://discord.gg/k4fuZtyDRu and sub to his YouTube: https://www.youtube.com/channel/UCy2259UHKx4awhMIkjT0lkQ

Spawns below types of Raptors (only one at each spawn) at Chicken Spawns & Bear Spawns on Chernarus:

dbo_raptor (medium size)
dbo_raptorB (Juvenile, small)
dbo_idrex (full size)
dbo_tricero (Big!)
dbo_trex (run!!!!)

THIS IS NOT DEANOSBEANO'S OFFICIAL INSTALL INSTRUCTIONS AND IS NOT AFFILIATED WITH DEANOBEANO.

Limited Testing on PC Chernarus Local Server & Nitrado Community PC Server DAYZ Version 1.15 Jan 2022.

XML snippets Created by @scalespeeder. Please report bugs & errors to scalespeeder@gmail.com with screenshots.

TERMS OF USE
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

PLEASE SEE THE README INSIDE THE DB-RAPTOR MOD FOR DEANOBEANO'S TERMS OF USE.

Using these modded xml / json files and instructions could break the functioning of your DAYZ server, requiring a reinstall that would wipe
all player progress.

Using these modded files neccessitates increased regular restarts to prevent server crashing.

It is suggested you thoroughly test your server after applying these files to ensure proper
functioning of your server.

I always recomend you validate your files at: https://www.xmlvalidation.com/ and https://jsonformatter.curiousconcept.com/

Instructions:

Subscribe to dbo_raptors mod on Steam:

https://steamcommunity.com/sharedfiles/filedetails/?id=2684950452

Start your DayZ Launcher to download the mod files. Using your FTP programme, copy the @dbo_raptors folder from your DayZ !workshop folder
to the root directory of your server. Copy the key from the mods key folder to your servers key folder. Edit your start batch file,
so that your server will load @dbo_raptors mod on startup. (On Nitrado and some other DayZ Server Providers you don't have access to the batch file,
instead you will find an "Additional mods" setting in the settings section of your servers web interface, add @dbo_raptors there.)

Click the "Code" button and "Download Zip" on the Github Repository and extract the files on your local PC for access.

Stop your server using it's web control panel.

Using FTP or your Servers file browser, upload the rap2and3_territories.xml to your servers env folder.

Open your events.xml file (its in the db folder on your server) and add the following XML snippet at the top, below the <events> tag:

<!--Bear Spawn Raptor1 entry-->
	<event name="AnimalRaptor1">
        <nominal>20</nominal>
        <min>20</min>
        <max>20</max>
        <lifetime>180</lifetime>
        <restock>0</restock>
        <saferadius>40</saferadius>
        <distanceradius>0</distanceradius>
        <cleanupradius>0</cleanupradius>
        <flags deletable="0" init_random="0" remove_damaged="1"/>
        <position>fixed</position>
        <limit>custom</limit>
        <active>1</active>
        <children>
            <child lootmax="0" lootmin="0" max="1" min="1" type="dbo_idrex"/>
        </children>
    </event>
    <!--Bear Spawn Raptor1B entry-->
	<event name="AnimalRaptor1B">
        <nominal>20</nominal>
        <min>20</min>
        <max>20</max>
        <lifetime>180</lifetime>
        <restock>0</restock>
        <saferadius>40</saferadius>
        <distanceradius>0</distanceradius>
        <cleanupradius>0</cleanupradius>
        <flags deletable="0" init_random="0" remove_damaged="1"/>
        <position>fixed</position>
        <limit>custom</limit>
        <active>1</active>
        <children>
            <child lootmax="0" lootmin="0" max="1" min="1" type="dbo_trex"/>
        </children>
    </event>
    <!--Bear Spawn Raptor1C entry-->
	<event name="AnimalRaptor1C">
        <nominal>20</nominal>
        <min>20</min>
        <max>20</max>
        <lifetime>180</lifetime>
        <restock>0</restock>
        <saferadius>40</saferadius>
        <distanceradius>0</distanceradius>
        <cleanupradius>0</cleanupradius>
        <flags deletable="0" init_random="0" remove_damaged="1"/>
        <position>fixed</position>
        <limit>custom</limit>
        <active>1</active>
        <children>
            <child lootmax="0" lootmin="0" max="1" min="1" type="dbo_tricero"/>
        </children>
    </event>
	<!--Hen Spawn Large Raptor2 entry-->
	<event name="AnimalRaptor2">
        <nominal>40</nominal>
        <min>40</min>
        <max>40</max>
        <lifetime>180</lifetime>
        <restock>0</restock>
        <saferadius>40</saferadius>
        <distanceradius>0</distanceradius>
        <cleanupradius>0</cleanupradius>
        <flags deletable="0" init_random="0" remove_damaged="1"/>
        <position>fixed</position>
        <limit>custom</limit>
        <active>1</active>
        <children>
            <child lootmax="0" lootmin="0" max="1" min="1" type="dbo_idrex"/>
        </children>
    </event>
	<!--Hen Spawn Small Raptor3 entry-->
	<event name="AnimalRaptor3">
        <nominal>40</nominal>
        <min>40</min>
        <max>40</max>
        <lifetime>180</lifetime>
        <restock>0</restock>
        <saferadius>40</saferadius>
        <distanceradius>0</distanceradius>
        <cleanupradius>0</cleanupradius>
        <flags deletable="0" init_random="0" remove_damaged="1"/>
        <position>fixed</position>
        <limit>custom</limit>
        <active>1</active>
        <children>
            <child lootmax="0" lootmin="0" max="1" min="1" type="dbo_raptor"/>
        </children>
    </event>
	<!--Hen Spawn Small Raptor4 entry-->
	<event name="AnimalRaptor4">
        <nominal>40</nominal>
        <min>40</min>
        <max>40</max>
        <lifetime>180</lifetime>
        <restock>0</restock>
        <saferadius>40</saferadius>
        <distanceradius>0</distanceradius>
        <cleanupradius>0</cleanupradius>
        <flags deletable="0" init_random="0" remove_damaged="1"/>
        <position>fixed</position>
        <limit>custom</limit>
        <active>1</active>
        <children>
            <child lootmax="0" lootmin="0" max="1" min="1" type="dbo_raptorB"/>
        </children>
    </event>
	
Save the file and re-upload if necessary.

Open your cfgenvironment.xml file (its in the root folder of the mission folder on your server) and add the following XML snippet,
just below "<file path="env/bear_territories.xml" />" which is near the top of the file:

		<!--raptor entry-->
		<file path="env/rap2and3_territories.xml" />
		
In the same file, but a little further down, add the following XML snippet,
just below "<territory type="Herd" name="Bear" behavior="BlissBearGroupBeh">
			<file usable="bear_territories"/>
			</territory>"

		<!--Bear Spawn Raptor1 entry-->
		<territory type="Herd" name="Raptor1" behavior="BlissBearGroupBeh">
			<file usable="bear_territories"/>
		</territory>
		<!--Bear Spawn Raptor1B entry-->
		<territory type="Herd" name="Raptor1B" behavior="BlissBearGroupBeh">
			<file usable="bear_territories"/>
		</territory>
		<!--Bear Spawn Raptor1C entry-->
		<territory type="Herd" name="Raptor1C" behavior="BlissBearGroupBeh">
			<file usable="bear_territories"/>
		</territory>
		<!--Hen Spawn Raptor2 entry-->
		<territory type="Herd" name="Raptor2" behavior="BlissBearGroupBeh">
			<file usable="rap2and3_territories"/>
		</territory>
		<!--Hen Spawn Raptor3 entry-->
		<territory type="Herd" name="Raptor3" behavior="BlissBearGroupBeh">
			<file usable="rap2and3_territories"/>
		</territory>
		<!--Hen Spawn Raptor4 entry-->
		<territory type="Herd" name="Raptor4" behavior="BlissBearGroupBeh">
			<file usable="rap2and3_territories"/>
		</territory>

Save your changes & upload if you need to.

Restart your server and the Raptors will be spawning in for the enjoyment of your players!!!!!

Thanks again to DEANOSBEANO

Please join his Discord: https://discord.gg/k4fuZtyDRu and / or sub to his YouTube: https://www.youtube.com/channel/UCy2259UHKx4awhMIkjT0lkQ

Thanks, Rob.
