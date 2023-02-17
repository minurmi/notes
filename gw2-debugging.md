# Trying to get GW1 to BLE loop

several times

Oct 07 14:10:22 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:22:INFO:Pairing...
Oct 07 14:10:28 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:28:INFO:RequestPasskey (/org/bluez/hci0/dev_C7_82_46_C2_2C_1E)
Oct 07 14:10:28 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:28:INFO:Trying to pair with the following passkey: 167511
Oct 07 14:10:29 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:29:INFO:Device paired
Oct 07 14:10:29 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:29:INFO:Paired to device: C7:82:46:C2:2C:1E
Oct 07 14:10:29 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:29:INFO:Connecting...
Oct 07 14:10:29 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:29:INFO:Connected to device: PulseOn AM-1
Oct 07 14:10:30 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:30:INFO:Subscribed notifications
Oct 07 14:10:30 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:30:INFO:Discovery Stopped
Oct 07 14:10:30 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:30:DEBUG:Flushing queue
Oct 07 14:10:30 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:30:DEBUG:Communication sent; type:2 retval:None data:bytearray(b'(\xa1\x00\x06\x00\x00')
Oct 07 14:10:30 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:30:WARNING:Exception: org.bluez.Error.Failed: Not connected
Oct 07 14:10:30 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:30:INFO:Unsubscribed notifications
Oct 07 14:10:30 treongw1-e66f5c0c python3[1850]: 2022-10-07 14:10:30:DEBUG:Communication sent; type:4 retval:None data:bytearray(b'')
Oct 07 14:10:30 treongw1-e66f5c0c python3[2070]: Delete bluetooth cache...
-------------------------

Oct 07 12:56:23 treongw1-e66f5c0c python3[889]: 2022-10-07 12:56:23:INFO:Pairing...
Oct 07 12:56:30 treongw1-e66f5c0c python3[889]: 2022-10-07 12:56:30:INFO:RequestPasskey (/org/bluez/hci0/dev_C7_82_46_C2_2C_1E)
Oct 07 12:56:30 treongw1-e66f5c0c python3[889]: 2022-10-07 12:56:30:INFO:Trying to pair with the following passkey: 167511
Oct 07 12:56:32 treongw1-e66f5c0c python3[889]: 2022-10-07 12:56:32:INFO:Device paired
Oct 07 12:56:33 treongw1-e66f5c0c python3[889]: 2022-10-07 12:56:33:INFO:Paired to device: C7:82:46:C2:2C:1E
Oct 07 12:56:33 treongw1-e66f5c0c python3[889]: 2022-10-07 12:56:33:INFO:Connecting...
Oct 07 12:56:33 treongw1-e66f5c0c python3[889]: 2022-10-07 12:56:33:INFO:Connected to device: PulseOn AM-1
Oct 07 12:56:34 treongw1-e66f5c0c python3[889]: 2022-10-07 12:56:34:INFO:Subscribed notifications
Oct 07 12:56:34 treongw1-e66f5c0c python3[889]: 2022-10-07 12:56:34:INFO:Discovery Stopped
Oct 07 12:56:34 treongw1-e66f5c0c python3[889]: 2022-10-07 12:56:34:DEBUG:Flushing queue
Oct 07 12:56:34 treongw1-e66f5c0c python3[889]: 2022-10-07 12:56:34:DEBUG:Communication sent; type:2 retval:None data:bytearray(b'-\xa1\x00\x06\x00\x00')
Oct 07 12:58:04 treongw1-e66f5c0c python3[889]: 2022-10-07 12:58:04:WARNING:We did not get all the data!
Oct 07 12:58:04 treongw1-e66f5c0c python3[889]: 2022-10-07 12:58:04:DEBUG:Flushing queue
Oct 07 12:58:04 treongw1-e66f5c0c python3[889]: 2022-10-07 12:58:04:WARNING:Resend message failed 2 times. Restart loop.
Oct 07 12:58:04 treongw1-e66f5c0c python3[889]: 2022-10-07 12:58:04:INFO:Next cycle start in 60 seconds
Oct 07 12:59:04 treongw1-e66f5c0c python3[889]: 2022-10-07 12:59:04:DEBUG:Communication sent; type:4 retval:None data:bytearray(b'')
Oct 07 12:59:04 treongw1-e66f5c0c python3[1306]: Delete bluetooth cache...

-------------------------

Oct 07 13:11:56 treongw1-e66f5c0c python3[889]: 2022-10-07 13:11:56:INFO:Pairing...
Oct 07 13:11:58 treongw1-e66f5c0c python3[889]: 2022-10-07 13:11:58:INFO:RequestPasskey (/org/bluez/hci0/dev_C7_82_46_C2_2C_1E)
Oct 07 13:11:58 treongw1-e66f5c0c python3[889]: 2022-10-07 13:11:58:INFO:Trying to pair with the following passkey: 167511
Oct 07 13:11:59 treongw1-e66f5c0c python3[889]: 2022-10-07 13:11:59:INFO:Device paired
Oct 07 13:11:59 treongw1-e66f5c0c python3[889]: 2022-10-07 13:11:59:INFO:Paired to device: C7:82:46:C2:2C:1E
Oct 07 13:11:59 treongw1-e66f5c0c python3[889]: 2022-10-07 13:11:59:INFO:Connecting...
Oct 07 13:11:59 treongw1-e66f5c0c python3[889]: 2022-10-07 13:11:59:INFO:Connected to device: PulseOn AM-1
Oct 07 13:11:59 treongw1-e66f5c0c python3[889]: 2022-10-07 13:11:59:INFO:Subscribed notifications
Oct 07 13:11:59 treongw1-e66f5c0c python3[889]: 2022-10-07 13:11:59:INFO:Discovery Stopped
Oct 07 13:11:59 treongw1-e66f5c0c python3[889]: 2022-10-07 13:11:59:DEBUG:Flushing queue
Oct 07 13:11:59 treongw1-e66f5c0c python3[889]: 2022-10-07 13:11:59:DEBUG:Communication sent; type:2 retval:None data:bytearray(b' \xa1\x00\x06\x00\x00')
Oct 07 13:12:00 treongw1-e66f5c0c python3[889]: 2022-10-07 13:12:00:INFO:Succesful hand shake!
Oct 07 13:12:00 treongw1-e66f5c0c python3[889]: 2022-10-07 13:12:00:DEBUG:Handle command. Type: 1 Params: [0, 4]
Oct 07 13:12:00 treongw1-e66f5c0c python3[889]: 2022-10-07 13:12:00:DEBUG:Communication sent; type:2 retval:None data:bytearray(b' \xa0\x00\x0b\x00\x00\x03\x04>
Oct 07 13:12:00 treongw1-e66f5c0c python3[889]: 2022-10-07 13:12:00:DEBUG:Handle command. Type: 1 Params: [0, 4]
Oct 07 13:12:00 treongw1-e66f5c0c python3[889]: 2022-10-07 13:12:00:WARNING:Control Field was not empty as it should be. Message bytearray(b' \xa3\x00\x06\x00\>

-------------------------

Oct 08 00:16:47 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:47:INFO:Pairing...
Oct 08 00:16:53 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:53:INFO:RequestPasskey (/org/bluez/hci0/dev_C7_82_46_C2_2C_1E)
Oct 08 00:16:53 treongw1-e66f5c0c systemd-journald[881]: Forwarding to syslog missed 25 messages.
Oct 08 00:16:53 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:53:INFO:Trying to pair with the following passkey: 167511
Oct 08 00:16:54 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:54:INFO:Device paired
Oct 08 00:16:54 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:54:INFO:Paired to device: C7:82:46:C2:2C:1E
Oct 08 00:16:54 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:54:INFO:Connecting...
Oct 08 00:16:54 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:54:INFO:Connected to device: PulseOn AM-1
Oct 08 00:16:54 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:54:INFO:Discovery Stopped
Oct 08 00:16:54 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:54:DEBUG:Flushing queue
Oct 08 00:16:54 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:54:DEBUG:Communication sent; type:2 retval:None data:bytearray(b')\xa1\x00\x06\x00\x00')
Oct 08 00:16:54 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:54:INFO:Subscribed notifications
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:INFO:Renegotiation of the connection ID
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:DEBUG:Flushing queue
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:WARNING:Message flushed: Type 2, RetVal 1, Data bytearray(b'*\xa1\x00\x06\x00\x00')
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:DEBUG:Communication sent; type:2 retval:None data:bytearray(b'*\xa1\x00\x06\x00\x00')
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:INFO:Succesful hand shake!
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:DEBUG:Handle command. Type: 1 Params: [0, 4]
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:DEBUG:Communication sent; type:2 retval:None data:bytearray(b'*\xa0\x00\x0b\x00\x00\x03\x0>
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:DEBUG:Handle command. Type: 1 Params: [0, 4]
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:WARNING:Control Field was not empty as it should be. Message bytearray(b'*\xa3\x00\x06\x00>
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:DEBUG:Handle command. Type: 1 Params: [0, 4]
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:DEBUG:Communication sent; type:2 retval:None data:bytearray(b'*\xa0\x00\x0b\x00\x05\x03\x0>
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:DEBUG:Handle command. Type: 1 Params: [0, 4]
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:INFO:Device UID: (01)06430054330121(10)0222(11)220121(21)000283
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:DEBUG:Handle command. Type: 2 Params: [1]
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:DEBUG:Communication sent; type:2 retval:None data:bytearray(b'*\xa0\x00\x14\x00\n\x0f\x00\>
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: 2022-10-08 00:16:55:DEBUG:Handle command. Type: 2 Params: [1]
Oct 08 00:16:55 treongw1-e66f5c0c python3[7956]: Uncaught exception
