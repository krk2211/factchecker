# factchecker
A simple fact checker. (NLP S6)

## Follow the setup instructions below.
1.  Clone the Repository.
    ```
    $ git clone https://github.com/krk2211/factchecker.git
    ```

2. Enter the folder.
    ```
    $ cd factchecker
    ```
3. Install python NLTK
    ```
	$ pip install nltk
    ```
4. Enter the sopex folder.
    ```
    $ cd sopex
    ```
4. Install Sopex
    ```
    $ python setup.py install
    ```
5. Install the required nltk modules.
    ```
    $ python
    >>> import nltk
    >>> nltk.download('punkt')
    >>> nltk.download('wordnet')
    ```
6. Run the code from sopex/script.py
    ```
    $ python script.py
    ```
7. The dataset is available in sopex/test.txt












    ### Source

        $ python setup.py install

    ### PyPI

        $ easy_install sopex

    ## Usage

    ### Help

    	$ sopex -h

    ### CLI

    	$ sopex "A rare black squirrel has become a regular visitor to a suburban garden"

    ### Library

        >>> import sopex
        >>> sentence = 'A rare black squirrel has become a regular visitor to a suburban garden'
        >>> triplet = sopex.extract(sentence)
        >>> print triplet.subject, triplet.predicate, triplet.object
