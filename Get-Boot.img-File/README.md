To extract the `boot.img` from an Android firmware payload.bin file using Payload Dumper, follow these steps:

1. **Set Up the Environment**:
    - Ensure you have Python installed on your system. If not, download and install it from [Python's official site](https://www.python.org/downloads/).
    - Install the necessary Python packages by running:
      ```bash
      pip install protobuf
      ```

2. **Download Payload Dumper**:
    - You can clone the Payload Dumper repository from GitHub:
      ```bash
      git clone https://github.com/vm03/payload_dumper.git
      ```
    - Navigate to the directory:
      ```bash
      cd payload_dumper
      ```

3. **Prepare the Payload.bin File**:
    - Ensure you have the `payload.bin` file from the OTA (Over-The-Air) update package.

4. **Extract the boot.img**:
    - Place the `payload.bin` file in the `payload_dumper` directory.
    - Run the Payload Dumper script:
      ```bash
      python payload_dumper.py payload.bin
      ```

5. **Locate the boot.img**:
    - Once the script finishes, it will create an `output` directory within the `payload_dumper` directory.
    - Inside this `output` directory, you will find the extracted `boot.img`.

### Detailed Steps:

1. **Install Python and protobuf**:
    ```bash
    sudo apt-get update
    sudo apt-get install python3 python3-pip
    pip3 install protobuf
    ```

2. **Clone the Payload Dumper repository**:
    ```bash
    git clone https://github.com/vm03/payload_dumper.git
    cd payload_dumper
    ```

3. **Place `payload.bin` in the directory**:
    Ensure `payload.bin` is in the `payload_dumper` directory.

4. **Run Payload Dumper**:
    ```bash
    python3 payload_dumper.py payload.bin
    ```

5. **Extracted Files**:
    After the script completes, navigate to the `output` directory to find `boot.img` along with other extracted images.

If you encounter any issues or need further assistance, feel free to ask!
