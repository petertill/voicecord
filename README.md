VoiceCord is a simple yet powerful voice recording package for Discord


Traceback (most recent call last):
  File "G:\projects\testing\main.py", line 7, in <module>
    asyncio.run(client.connect())
  File "C:\Users\tillp\miniconda\Lib\asyncio\runners.py", line 194, in run
    return runner.run(main)
           ^^^^^^^^^^^^^^^^
  File "C:\Users\tillp\miniconda\Lib\asyncio\runners.py", line 118, in run
    return self._loop.run_until_complete(task)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "C:\Users\tillp\miniconda\Lib\asyncio\base_events.py", line 684, in run_until_complete
    return future.result()
           ^^^^^^^^^^^^^^^
  File "C:\Users\tillp\miniconda\Lib\site-packages\voicecord\__init__.py", line 67, in connect
    await self.__listen_gateway(websocket)
  File "C:\Users\tillp\miniconda\Lib\site-packages\voicecord\__init__.py", line 149, in __listen_gateway
    await self.__voice_identify(websocket)
  File "C:\Users\tillp\miniconda\Lib\site-packages\voicecord\__init__.py", line 173, in __voice_identify
    await self.__listen_voice_server(self.VOICE_WS)
  File "C:\Users\tillp\miniconda\Lib\site-packages\voicecord\__init__.py", line 219, in __listen_voice_server
    asyncio.create_task(self.__heartbeat(interval, websocket))
                        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
TypeError: VoiceClient.__heartbeat() takes 2 positional arguments but 3 were given
Voice client destroyed