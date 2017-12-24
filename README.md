# google_map
a python script for searching a place through google map, enter the search string through command line or copy to clipboard



      import webbrowser,sys,pyperclip

      if len(sys.argv)>1:
                  address=' '.join(sys.argv[1:])
      else:
                  address=pyperclip.paste()
      webbrowser.open('https://www.google.com/maps/place/'+address)
