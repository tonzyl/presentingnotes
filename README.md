# presentingnotes
Take the presenter's notes from Keynote and put them on the clipboard.

The scpt file contains a simple apple script to copy all speaker notes from an active keynote presentation to the clipboard.

The script is: 
global spreeknotities
tell application "Keynote"
	tell front document
		set spreeknotities to presenter notes of every slide as text
		set the clipboard to spreeknotities
	end tell
end tell
