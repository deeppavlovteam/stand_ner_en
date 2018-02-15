# Demo stand. Model: NER (English)

## Installation and start
1. Clone the repo and `cd` to project root:
    ```
    git clone https://github.com/deepmipt/stand_ner_en.git
    cd stand_ner_en
    ```
2. Run script to download and unpack model components:
    ```
    ./download_components.sh
    ```   
3. Create a virtual environment with `Python 3.6`:
    ```
    virtualenv env -p python3.6
    ```
4. Activate the environment:
    ```
    source ./env/bin/activate
    ```
5. Install requirements:
    ```
    pip install -r requirements.txt
    ```
6. Download NLTK data:
    ```
    $ python3
    >>> import nltk
    >>> nltk.download('punkt')
    ```
7. Specify model endpoint host (`api_host`) and port (`api_port`) in `ner_agent_config.json`
7. Specify virtual environment path (if necessary) in `run_en_ner.sh`
8. Run model:
    ```
    ./run_en_ner.sh
    ```