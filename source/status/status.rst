.. _status:

Status
====================

The status endpoint can be called to verify that the API is up and running. It also provides the most recent release date and version of the Gamelocker service itself.

The following command can be used to call the status endpoint:

.. code-block:: shell

	curl -g "https://api.dc01.gamelockerapp.com/status" 
	-H "Authorization: Bearer <api key>" 
	-H "Accept: application/vnd.api+json"

The above command will return the following JSON:

.. code-block:: none

  {
    "data": {
      "type": "status",
      "id": "gamelocker",
      "attributes": {
        "releasedAt": "2017-11-22T20:25:05Z",
        "version": "v7.5.1"
      }
    }
  }


.. toctree::
  :maxdepth: 2
