# ImageEngine

ImageEngine is a Python package that allows users to search and download images from multiple sources such as DuckDuckGo, Bing, and Google. With a simple interface and command-line tools, you can easily obtain images of any search term.

## Features

- **Search DuckDuckGo**: Download images using the DuckDuckGo search engine.
- **Search Bing**: Download images using the Bing search engine.
- **Search Google, DuckDuckGo, and Bing**: Download images from all three search engines with a single command.

## Installation

To install the package, run:


```bash
pip install ImageEngine
```

Alternatively, you can clone the repository and install it locally:

```bash
git clone https://github.com/jaypunekar/ImageEngine.git
cd ImageEngine
pip install .
```

## Usage

### Command Line Interface (CLI)

After installing the package, you can use the following commands from your terminal:

1. **Search and download images from DuckDuckGo**:

   ```bash
   # "cute puppies" is the search string and "puppy_images" is the directory where images will be stored
   search-ddg term="cute puppies" path="puppy_images" --max_images=10
   ```

2. **Search and download images from Bing**:

   ```bash
   search-bing term="beautiful landscapes" path="landscapes" --max_images=20
   ```

3. **Search and download images from Google, DuckDuckGo, and Bing**:

   ```bash
   search-web term="happy animals" path="animals" --max_images=30
   ```

### Using Functions in Python Scripts

You can also import the functions directly in your Python scripts:

```python
from ImageEngine import searchDDG
from ImageEngine import searchBing
from ImageEngine import searchGoogle
from ImageEngine import searchWeb

# Search images from DuckDuckGo
# "sunset" is the search string and "sunset_images" is the directory where images will be stored
searchDDG(term="sunsets", path="sunset_images", max_images=10)

# Search images from Bing
searchBing(term="mountain views", path="mountain_images", max_images=15)

# Search images from Google
searchGoogle(term="river views", path="river_images", max_images=15)

# Search images from all three engines
searchWeb(term="cute cats", path="cat_images", max_images=20)
```

## Requirements

- Python 3.6 or higher
- `duckduckgo_search`
- `fastai`
- `icrawler`
- Other dependencies listed in `setup.py`

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request to contribute.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Contact

For any inquiries or issues, please contact [jay.punekar@icloud.com](mailto:jay.punekar@icloud.com).

