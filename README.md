# virtuale-dl

Extremely simple script to download every file of a course or multiple courses from https://virtuale.unibo.it

### Usage

The script needs the IDs of the courses, session cookies and the path where the
directories will be downloaded. You can either set them from command line with
options or editing the script directly.
```
Usage: ./virtuale-dl.sh [-c COOKIES] [-i COURSE_IDS] [-d DIR]
```
You can get the cookies in the right format by copying the request for
curl from the browser and then getting the `Cookie:` part of the header.

Example: `"Cookie: ApplicationGatewayAffinity=02138802938409f092;
MoodleSession=92837492834029384d;
_shibsession_6465666019283019283019287019238=_029984029384026383039384"`

For the `COURSE_IDS` variable use one or more IDs of the courses you want to
download files from, you can get them from the URL of the course. For example
the ID on https://virtuale.unibo.it/course/view.php?id=112233 is `112233`. 
You can specify more to download files from more courses. (i.e. `ID="112233 223344"`)

Finally the `DIR` variable sets the path where the downloaded directories will be stored.

