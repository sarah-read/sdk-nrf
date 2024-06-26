.. _ug_wifi_mem_req_sta_mode:

Memory requirements for Wi-Fi applications in Station mode
##########################################################

Code and RAM memory footprint requirements differ depending on the selected platform and the application example.

The following tables list memory requirement values for selected Wi-Fi® samples supporting Station mode.

Footprint values are provided in kilobytes (KB).

.. tabs::

   .. tab:: nRF52840 DK

      The following table lists memory requirements for sample running on the :ref:`nRF52840 DK <programming_board_names>` (:ref:`nrf52840dk/nrf52840 <zephyr:nrf52840dk_nrf52840>`).

      +--------------------------------------+-------------+-------------------------------------------+-----------------------------+----------------------+---------------------------------+--------------------+----------------------+
      | Sample                               |   Total ROM |   Wi-Fi driver ROM                        |          nRF70 FW patch ROM |   WPA supplicant ROM |   Total RAM (incl. static heap) |   Wi-Fi driver RAM |   WPA supplicant RAM |
      +======================================+=============+===========================================+=============================+======================+=================================+====================+======================+
      | :ref:`Station <wifi_station_sample>` |         502 |                                        51 |                          69 |                  180 |                             253 |                164 |                   11 |
      +--------------------------------------+-------------+-------------------------------------------+-----------------------------+----------------------+---------------------------------+--------------------+----------------------+

   .. tab:: nRF7002 DK

      The following table lists memory requirements for samples running on the :ref:`nRF7002 DK <programming_board_names>` (:ref:`nrf7002dk/nrf5340/cpuapp <nrf7002dk_nrf5340>`).

      +-----------------------------------------------+-------------+-------------------------------------------+-------------------------------+----------------------+---------------------------------+--------------------+----------------------+
      | Sample                                        |   Total ROM |   Wi-Fi driver ROM                        |            nRF70 FW patch ROM |   WPA supplicant ROM |   Total RAM (incl. static heap) |   Wi-Fi driver RAM |   WPA supplicant RAM |
      +===============================================+=============+===========================================+===============================+======================+=================================+====================+======================+
      | :ref:`UDP <udp_sample>`                       |         502 |                                        54 |                            69 |                  178 |                             214 |                101 |                   13 |
      +-----------------------------------------------+-------------+-------------------------------------------+-------------------------------+----------------------+---------------------------------+--------------------+----------------------+
      | :ref:`Station <wifi_station_sample>`          |         499 |                                        53 |                            69 |                  180 |                             254 |                164 |                   13 |
      +-----------------------------------------------+-------------+-------------------------------------------+-------------------------------+----------------------+---------------------------------+--------------------+----------------------+
      | :ref:`AWS IoT <aws_iot>`                      |         693 |                                        53 |                            69 |                  233 |                             305 |                101 |                   13 |
      +-----------------------------------------------+-------------+-------------------------------------------+-------------------------------+----------------------+---------------------------------+--------------------+----------------------+
      | :ref:`CoAP Client <net_coap_client_sample>`   |         590 |                                        55 |                            69 |                  178 |                             291 |                170 |                   13 |
      +-----------------------------------------------+-------------+-------------------------------------------+-------------------------------+----------------------+---------------------------------+--------------------+----------------------+
      | :ref:`HTTP Server <http_server>`              |         640 |                                        55 |                            69 |                  180 |                             273 |                121 |                   13 |
      +-----------------------------------------------+-------------+-------------------------------------------+-------------------------------+----------------------+---------------------------------+--------------------+----------------------+
      | :ref:`HTTPS Client <https_client>`            |         631 |                                        54 |                            69 |                  239 |                             281 |                101 |                   13 |
      +-----------------------------------------------+-------------+-------------------------------------------+-------------------------------+----------------------+---------------------------------+--------------------+----------------------+
      | :ref:`MQTT <mqtt_sample>`                     |         690 |                                        55 |                            69 |                  239 |                             309 |                101 |                   13 |
      +-----------------------------------------------+-------------+-------------------------------------------+-------------------------------+----------------------+---------------------------------+--------------------+----------------------+

      .. note::

         The footprint of the networking samples for the Zephyr image is derived from the board target with :ref:`Cortex-M Security Extensions enabled <app_boards_spe_nspe_cpuapp_ns>` (``*/ns`` :ref:`variant <app_boards_names>`).
