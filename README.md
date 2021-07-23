# AutomapperPerformance
This project to illustrate the difference in performance between the automapper and the manual mapper

Results:

AutoMapper with 1: 24
Manual Map with 1: 0

AutoMapper with 10: 0
Manual Map with 10: 0

AutoMapper with 100: 1
Manual Map with 100: 0

AutoMapper with 1000: 18
Manual Map with 1000: 0

AutoMapper with 10000: 112
Manual Map with 10000: 1

AutoMapper with 100000: 1070
Manual Map with 100000: 14

This shows:

While Automapper is constantly slower, I won't see the difference if the list is fewer than 1,000 entries. There are obvious slowdowns if my list is in the 10,000+ range. These are probably edge-cases that can be dealt with later, but I believe it's reasonable to assume that Automapper in a 'average' project won't obstruct you too much and will save you from writing a lot of code!
