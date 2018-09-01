[![Build Status](https://travis-ci.org/Marwolf/VolUtility-Docker.svg?branch=master)](https://travis-ci.org/Marwolf/VolUtility-Docker)

# VolUtility
Web Interface for Volatility Memory Analysis framework.

## Requirements:
 * Docker
 * Docker-Compose

## How To Use:
 * Copy a Volatility-accepted memory dump into the "memory-dump" directory
 * When adding your memory image, specify a location of "/opt/images/<your_memory_dump_filename>"
 * Add your VirusTotal API key in "volutility.conf"
 * Plugins specified in "volutility.conf" will automatically be ran against the memory dump with Volatility
 * Yara rules have been cloned from the official repository in the "yararules" directory, check for updates via "git pull"
 * Execute "Start.sh"
 * Visit http://localhost:8080

## Overview
Runs plugins and stores the output in a mongo database.
Extracts files from plugins (that support dump-dir) and stores them in the database
Search across all plugins and file content with string search and yara rules.
Allows you to work on multiple images in one database

Video Demo showing some of the features.
https://www.youtube.com/watch?v=ruEj94Zhn6I

## Wiki

See the wiki pages for detailed installation and usage details.

https://github.com/kevthehermit/VolUtility/wiki
