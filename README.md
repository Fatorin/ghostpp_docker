# Ghost++ Docker

Use guide:
1.Create "config" folder.
2.Put your settings file in "config" folder. (Main config name must be ghost.cfg, map.cfg has follow your ghost.cfg)
3.Put your map in "maps" folder.
4.Modify under line cmd to your real open port in ghost.cfg.

docker run -it -p 6113-6114:6113-6114 -v /config:/config --name ghostpp fatorin/ghostpp:1.2