# dev-starter-kit
A developer-friendly starter kit with best practices and structure
#!/usr/bin/env python3
"""
tamom-zendegi — Professional Starter Script
"""

import logging
import json
from pathlib import Path

# -------------------- CONFIGURATION --------------------
CONFIG_FILE = Path(__file__).parent / "config.json"

DEFAULT_CONFIG = {
    "project_name": "tamom-zendegi",
    "version": "1.0.0",
    "author": "Your Name",
    "welcome_message": "Hello! This is tamom-zendegi 🚀"
}

def load_config():
    """Load configuration from file or use default."""
    if CONFIG_FILE.exists():
        with open(CONFIG_FILE, "r", encoding="utf-8") as f:
            return json.load(f)
    else:
        return DEFAULT_CONFIG

# -------------------- LOGGING SETUP --------------------
def setup_logger():
    """Configure logger with nice formatting."""
    logging.basicConfig(
        level=logging.INFO,
        format="%(asctime)s | %(levelname)-8s | %(message)s",
        datefmt="%Y-%m-%d %H:%M:%S"
    )

# -------------------- MAIN FUNCTION --------------------

    "version": "1.0.0",
    "author": "Mojtaba",
    "welcome_message": "Welcome to tamom-zendegi — clean, structured, ready to grow 🚀"
}

