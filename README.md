# Automation Test
Instructions

System requirements
Node.js 18+
Windows 10+, Windows Server 2016+ or Windows Subsystem for Linux (WSL).
macOS 13 Ventura, or macOS 14 Sonoma.
Debian 11, Debian 12, Ubuntu 20.04 or Ubuntu 22.04, Ubuntu 24.04, on x86-64 and arm64 architecture.

1. Download the project there will be a WinRAR file with a folder named "Auto" inside it, extract the folder to anywhere.

2. Install / Use VSCode or any IDE tools make sure you have Node.js at least version 18.

3. Open the project folder (named: "Auto"), To install playwright, Run one of these commands in terminal (Skip if you have already done):
	[npm]
	npm init playwright@latest 
	[yarn]
	yarn create playwright
	[pnpm]
	pnpm create playwright

4. The "tests" Folder is where the tests are in and the only file in it(autotest.spec.js)
	should have 5 test cases according to the exam,
	you can config the test by going to playwright.config.js mainly on the line headless: false
	you can set it to true if you don't want to see the browser screens.

	There will be a folder named setups with a file named "variableSetUps"
	it uses for providing the test data for referring to some specified variables such as username and password.

5. The tests are already done and all have "Pass" Status with a screenshot on each step of the test in .png format
	You can view them in the project folder.

6. To run automated tests use this command
	npx playwright test
	It should run 15 tests as 5 tests are given to each browser and we have 3 browsers in total.
	The test will be screenshoted on every step, you can remove all of the png test result files to see the changes.

7. To View the result use this command
	npx playwright show-report
	It will open the browser with the test report and status.
	
