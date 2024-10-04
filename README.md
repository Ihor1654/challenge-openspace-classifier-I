# OpenSpace Organizer
[![forthebadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)


## 🏢 Description

Your company moved to a new office at the Gent Zuiderport. Its an openspace with 6 tables of 4 seats. As many of you are new colleagues, you come up with the idea of changing seats everyday and get to know each other better by working side by side with your new colleagues. 

This script runs everyday to re-assign everybody to a new seat.

![coworking_img](https://images.unsplash.com/photo-1519389950473-47ba0277781c?w=600&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8NDd8fGRpdmVyc2UlMjB0ZWFtfGVufDB8fDB8fHwy)

## 📦 Repo structure

```
.
├── utils/
│   ├── openspace.py
│   ├── table.py
│   └── file_utils.py
├── .gitignore
├── main.py
├── new_colleagues.csv
├── output.xlsx
├── requirements.txt
└── README.md
```

## Installation



## 🛎️ Usage

1. Clone the repository to your local machine.

2 .To run the script, you can execute the `main.py` file from your command line:

    ```
    python main.py
    ```

3. The script provides options to set up the open space capacity or runs with the default setting (6 tables with 4 seats each). It asks you to choose a .csv input file from your local machine and organizes your colleagues into random seat assignments. The resulting seating plan is displayed in your console and also saved to a file with a name you enter and a format you choose (.xlsx or .csv) in your root directory.

```python
classroom = ask_about_size()
classroom.organize(read_from_csv())
classroom.dysplay()
ask_filename()
```
4. The script also provides the ability to handle a lack of seats in the open space. It will ask you to input 'S', 'T', 'N' or 'B':
* 'T': add one table, 
* 'S': add one seat for each table, 
* 'B': add one table or add one seat to each table, 
* 'N': do nothing

5. And the option to add extra people, not included in the .csv, before saving the resulting seat map to the file.
* "Do you want to add somebody? Y/N"
    * 'Y' : answer yes
    * 'N' : answer no
* 'Write the names. if all names were added write E'
    * 'E' : stop adding the names         

## ⏱️ Timeline

This project took two days for completion.

## Contributors



## 📌 Personal Situation
This project was done as part of the AI Boocamp at BeCode.org. 

Connect with me on [LinkedIn](www.linkedin.com/in/ihor-afanasiev-a50798268).
