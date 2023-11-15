.PHONY: make_keymap_keebio_iris_rev6 copy_keymap_keebio_iris_rev6 compile_firmware_keebio_iris_rev6 run_iris_rev6 make_keymap setup_qmk copy_keymap compile_firmware copy_firmware clean

clean:
	cd .. && rm -rf .build
	cd .. *.hex

make_keymap_keebio_iris_rev6:
	cd .. && qmk json2c personal/keebio_iris_rev6/keymap.json -o personal/keebio_iris_rev6/keymap.c
	rm keebio_iris_rev6/keymap.c.bak

copy_keymap_keebio_iris_rev6:
	cd .. && cp -r personal/keebio_iris_rev6/* keyboards/keebio/iris/keymaps/personal

compile_firmware_keebio_iris_rev6:
	cd .. && qmk compile -kb keebio/iris/rev6 -km personal

flash_firmware_keebio_iris_rev6:
	cd .. && qmk flash -kb keebio/iris/rev6 -km personal

run_iris_rev6: clean make_keymap_keebio_iris_rev6 copy_keymap_keebio_iris_rev6 compile_firmware_keebio_iris_rev6

flash_iris_rev6: clean make_keymap_keebio_iris_rev6 copy_keymap_keebio_iris_rev6 flash_firmware_keebio_iris_rev6

make_keymap_keebio_iris_rev7:
	cd .. && qmk json2c personal/keebio_iris_rev7/keymap.json -o personal/keebio_iris_rev7/keymap.c
	rm keebio_iris_rev7/keymap.c.bak

copy_keymap_keebio_iris_rev7:
	cd .. && cp -r personal/keebio_iris_rev7/* keyboards/keebio/iris/keymaps/personal

compile_firmware_keebio_iris_rev7:
	cd .. && qmk compile -kb keebio/iris/rev7 -km personal

flash_firmware_keebio_iris_rev7:
	cd .. && qmk flash -kb keebio/iris/rev7 -km personal

run_iris_rev7: clean make_keymap_keebio_iris_rev7 copy_keymap_keebio_iris_rev7 compile_firmware_keebio_iris_rev7

flash_iris_rev7: clean make_keymap_keebio_iris_rev7 copy_keymap_keebio_iris_rev7 flash_firmware_keebio_iris_rev7

flash_pageturner:
	cd .. && qmk flash -kb pageturner -km default

make_keymap_piantor_pro:
	cd .. && qmk json2c personal/piantor_pro/keymap.json -o personal/piantor_pro/keymap.c
	rm piantor_pro/keymap.c.bak

copy_keymap_piantor_pro:
	cd .. && cp -r personal/piantor_pro/* keyboards/beekeeb/piantor_pro/keymaps/personal

compile_firmware_piantor_pro:
	cd .. && qmk compile -kb beekeeb/piantor_pro -km personal

flash_firmware_piantor_pro:
	cd .. && qmk flash -kb beekeeb/piantor_pro -km personal

run_piantor_pro: clean make_keymap_piantor_pro copy_keymap_piantor_pro compile_firmware_piantor_pro

flash_piantor_pro: clean make_keymap_piantor_pro copy_keymap_piantor_pro flash_firmware_piantor_pro
