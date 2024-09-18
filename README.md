
 •	Nmap: Install via your package manager (example for Ubuntu/Debian):

sudo apt install nmap



Clone the Repository

	1.	Clone the repository:

git clone https://github.com/kdairatchi/MultiToolV3


	2.	Navigate into the project directory:

cd MultiToolV3



Install Python Dependencies

	1.	Install the required Python packages:

pip install -r requirements.txt


	2.	Install tkinter (required for the GUI version):

sudo apt install python3-tk



Usage

Command-Line Version

To use the command-line version of the tool:

	1.	Run the script with a target IP or domain:

python3 MultiToolCLI.py <target>


	2.	After running the command, you’ll be prompted to select a tool for scanning:
	•	1 for Naabu
	•	2 for Nmap
	•	3 for Scapy

Example:

python3 MultiToolCLI.py 192.168.1.1

GUI Version

To use the graphical interface version:

	1.	Run the GUI script:

python3 MultiToolGUI.py


	2.	You’ll see a window where you can:
	•	Select a tool (Naabu, Nmap, or Scapy)
	•	Enter the target IP or domain
	•	Press Scan to initiate the scan

Requirements

	•	Python 3.x
	•	Naabu
	•	Nmap
	•	Scapy
	•	Tkinter (for GUI)

To install the dependencies, refer to the Installation section above.

Troubleshooting

Naabu Not Found

If you encounter an error saying naabu: command not found, ensure Naabu is correctly installed and added to your PATH. To verify Naabu installation:

naabu -version

If Naabu isn’t installed, use:

go install -v github.com/projectdiscovery/naabu/v2/cmd/naabu@latest

Scapy Import Error

If you see an error related to Scapy not being installed:

ImportError: No module named scapy

Install Scapy using pip:

pip install scapy

GUI Issues

If you encounter issues with the GUI version (such as tkinter not found), ensure Tkinter is installed:

sudo apt install python3-tk

License

This project is licensed under the MIT License - see the LICENSE file for details.

Contributing

Feel free to contribute to this project by submitting issues or pull requests. For major changes, please open an issue first to discuss what you would like to change.

Contact

Created by kdairatchi. If you have any questions or feedback, feel free to reach out!

---

## 4. **Additional Instructions**

### **Make the Scripts Executable**

To make the scripts easier to run, you can set the Python scripts as executable:

```bash
chmod +x MultiToolCLI.py
chmod +x MultiToolGUI.py

Now, you can run the scripts directly:

./MultiToolCLI.py <target>
./MultiToolGUI.py

This guide should cover all aspects of setting up, running, and troubleshooting the Multi-Tool Network Scanner project. You can customize the repository, modify the README.md, and make necessary updates as you see fit.
