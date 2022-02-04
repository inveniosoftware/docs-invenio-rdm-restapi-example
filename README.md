# InvenioRDM REST API Example

Following is an example of how to programmatically upload a record to an
InvenioRDM.

In the example, we will use the InvenioRDM demo site hosted on
https://inveniordm.web.cern.ch/, you can as well just


## Requirements

You'll need Python and the requests library:

```
pip install requests
```

## Obtain a token

You need to obtain an access token, by creating one here:

- https://inveniordm.web.cern.ch/account/settings/applications/tokens/new/

Next, edit [``upload.py``](upload.py) and add the token:

```python
api = "https://inveniordm.web.cern.ch"
token = "<insert token here>"
```

### Files

- ``record.json`` - the record metadata JSON file.
- ``1911.00295.pdf`` - the record data file.

## Running

You can run the upload script using Python:

```
python upload.py
```
