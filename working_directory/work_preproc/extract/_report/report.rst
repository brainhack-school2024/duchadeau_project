Node: extract (fsl)
===================


 Hierarchy : work_preproc.extract
 Exec ID : extract


Original Inputs
---------------


* args : <undefined>
* center : <undefined>
* environ : {'FSLOUTPUTTYPE': 'NIFTI_GZ'}
* frac : <undefined>
* functional : <undefined>
* in_file : /home/rduchadeau/Desktop/Brainhack_school/duchadeau_project/working_directory/work_preproc/extract/sub-01_task-rest_run-1_bold_redresse.nii
* mask : <undefined>
* mesh : <undefined>
* no_output : <undefined>
* out_file : output_brain.nii.gz
* outline : <undefined>
* output_type : NIFTI_GZ
* padding : <undefined>
* radius : <undefined>
* reduce_bias : <undefined>
* remove_eyes : <undefined>
* robust : <undefined>
* skull : <undefined>
* surfaces : <undefined>
* t2_guided : <undefined>
* threshold : <undefined>
* vertical_gradient : <undefined>


Execution Inputs
----------------


* args : <undefined>
* center : <undefined>
* environ : {'FSLOUTPUTTYPE': 'NIFTI_GZ'}
* frac : <undefined>
* functional : <undefined>
* in_file : /home/rduchadeau/Desktop/Brainhack_school/duchadeau_project/working_directory/work_preproc/extract/sub-01_task-rest_run-1_bold_redresse.nii
* mask : <undefined>
* mesh : <undefined>
* no_output : <undefined>
* out_file : output_brain.nii.gz
* outline : <undefined>
* output_type : NIFTI_GZ
* padding : <undefined>
* radius : <undefined>
* reduce_bias : <undefined>
* remove_eyes : <undefined>
* robust : <undefined>
* skull : <undefined>
* surfaces : <undefined>
* t2_guided : <undefined>
* threshold : <undefined>
* vertical_gradient : <undefined>


Execution Outputs
-----------------


* inskull_mask_file : <undefined>
* inskull_mesh_file : <undefined>
* mask_file : <undefined>
* meshfile : <undefined>
* out_file : /home/rduchadeau/Desktop/Brainhack_school/duchadeau_project/working_directory/work_preproc/extract/output_brain.nii.gz
* outline_file : <undefined>
* outskin_mask_file : <undefined>
* outskin_mesh_file : <undefined>
* outskull_mask_file : <undefined>
* outskull_mesh_file : <undefined>
* skull_file : <undefined>
* skull_mask_file : <undefined>


Runtime info
------------


* cmdline : bet sub-01_task-rest_run-1_bold_redresse.nii output_brain.nii.gz
* duration : 3.082689
* hostname : BOOK-Romain
* prev_wd : /home/rduchadeau/Desktop/Brainhack_school/duchadeau_project
* working_dir : /home/rduchadeau/Desktop/Brainhack_school/duchadeau_project/working_directory/work_preproc/extract


Terminal output
~~~~~~~~~~~~~~~


 


Terminal - standard output
~~~~~~~~~~~~~~~~~~~~~~~~~~


 


Terminal - standard error
~~~~~~~~~~~~~~~~~~~~~~~~~


 


Environment
~~~~~~~~~~~


* APPLICATION_INSIGHTS_NO_DIAGNOSTIC_CHANNEL : 1
* CLICOLOR : 1
* CLICOLOR_FORCE : 1
* CONDA_DEFAULT_ENV : base
* CONDA_EXE : /home/rduchadeau/miniconda3/bin/conda
* CONDA_PREFIX : /home/rduchadeau/miniconda3
* CONDA_PROMPT_MODIFIER : (base) 
* CONDA_PYTHON_EXE : /home/rduchadeau/miniconda3/bin/python
* CONDA_ROOT : /home/rduchadeau/miniconda3
* CONDA_SHLVL : 1
* DBUS_SESSION_BUS_ADDRESS : unix:path=/run/user/1000/bus
* DISPLAY : :0
* ELECTRON_RUN_AS_NODE : 1
* FORCE_COLOR : 1
* FSLDIR : /home/rduchadeau/fsl
* FSLMULTIFILEQUIT : TRUE
* FSLOUTPUTTYPE : NIFTI_GZ
* FSLTCLSH : /home/rduchadeau/fsl/bin/fsltclsh
* FSLWISH : /home/rduchadeau/fsl/bin/fslwish
* FSL_LOAD_NIFTI_EXTENSIONS : 0
* FSL_SKIP_GLOBAL : 0
* GIT_PAGER : cat
* GSETTINGS_SCHEMA_DIR : /home/rduchadeau/miniconda3/share/glib-2.0/schemas
* GSETTINGS_SCHEMA_DIR_CONDA_BACKUP : 
* HOME : /home/rduchadeau
* HOSTTYPE : x86_64
* LANG : C.UTF-8
* LESSCLOSE : /usr/bin/lesspipe %s %s
* LESSOPEN : | /usr/bin/lesspipe %s
* LOGNAME : rduchadeau
* LS_COLORS : rs=0:di=01;34:ln=01;36:mh=00:pi=40;33:so=01;35:do=01;35:bd=40;33;01:cd=40;33;01:or=40;31;01:mi=00:su=37;41:sg=30;43:ca=30;41:tw=30;42:ow=34;42:st=37;44:ex=01;32:*.tar=01;31:*.tgz=01;31:*.arc=01;31:*.arj=01;31:*.taz=01;31:*.lha=01;31:*.lz4=01;31:*.lzh=01;31:*.lzma=01;31:*.tlz=01;31:*.txz=01;31:*.tzo=01;31:*.t7z=01;31:*.zip=01;31:*.z=01;31:*.dz=01;31:*.gz=01;31:*.lrz=01;31:*.lz=01;31:*.lzo=01;31:*.xz=01;31:*.zst=01;31:*.tzst=01;31:*.bz2=01;31:*.bz=01;31:*.tbz=01;31:*.tbz2=01;31:*.tz=01;31:*.deb=01;31:*.rpm=01;31:*.jar=01;31:*.war=01;31:*.ear=01;31:*.sar=01;31:*.rar=01;31:*.alz=01;31:*.ace=01;31:*.zoo=01;31:*.cpio=01;31:*.7z=01;31:*.rz=01;31:*.cab=01;31:*.wim=01;31:*.swm=01;31:*.dwm=01;31:*.esd=01;31:*.jpg=01;35:*.jpeg=01;35:*.mjpg=01;35:*.mjpeg=01;35:*.gif=01;35:*.bmp=01;35:*.pbm=01;35:*.pgm=01;35:*.ppm=01;35:*.tga=01;35:*.xbm=01;35:*.xpm=01;35:*.tif=01;35:*.tiff=01;35:*.png=01;35:*.svg=01;35:*.svgz=01;35:*.mng=01;35:*.pcx=01;35:*.mov=01;35:*.mpg=01;35:*.mpeg=01;35:*.m2v=01;35:*.mkv=01;35:*.webm=01;35:*.webp=01;35:*.ogm=01;35:*.mp4=01;35:*.m4v=01;35:*.mp4v=01;35:*.vob=01;35:*.qt=01;35:*.nuv=01;35:*.wmv=01;35:*.asf=01;35:*.rm=01;35:*.rmvb=01;35:*.flc=01;35:*.avi=01;35:*.fli=01;35:*.flv=01;35:*.gl=01;35:*.dl=01;35:*.xcf=01;35:*.xwd=01;35:*.yuv=01;35:*.cgm=01;35:*.emf=01;35:*.ogv=01;35:*.ogx=01;35:*.aac=00;36:*.au=00;36:*.flac=00;36:*.m4a=00;36:*.mid=00;36:*.midi=00;36:*.mka=00;36:*.mp3=00;36:*.mpc=00;36:*.ogg=00;36:*.ra=00;36:*.wav=00;36:*.oga=00;36:*.opus=00;36:*.spx=00;36:*.xspf=00;36:
* MPLBACKEND : module://matplotlib_inline.backend_inline
* NAME : Code
* PAGER : cat
* PATH : /home/rduchadeau/miniconda3/bin:/home/rduchadeau/.vscode-server/bin/dc96b837cf6bb4af9cd736aa3af08cf8279f7685/bin/remote-cli:/home/rduchadeau/fsl/share/fsl/bin:/home/rduchadeau/fsl/share/fsl/bin:/home/rduchadeau/miniconda3/bin:/home/rduchadeau/miniconda3/condabin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/usr/lib/wsl/lib:/mnt/c/Program Files (x86)/VMware/VMware Player/bin:/mnt/c/windows/system32:/mnt/c/windows:/mnt/c/windows/System32/Wbem:/mnt/c/windows/System32/WindowsPowerShell/v1.0:/mnt/c/windows/System32/OpenSSH:/mnt/c/Program Files/Git/cmd:/mnt/c/Program Files/MATLAB/MATLAB Runtime/R2023b/runtime/win64:/Docker/host/bin:/mnt/c/Users/romai/AppData/Local/Microsoft/WindowsApps:/mnt/c/Users/romai/AppData/Local/Programs/Microsoft VS Code/bin:/mnt/c/msys64/ucrt64/bin:/snap/bin
* PULSE_SERVER : unix:/mnt/wslg/PulseServer
* PWD : /mnt/c/Users/romai/AppData/Local/Programs/Microsoft VS Code
* PYDEVD_IPYTHON_COMPATIBLE_DEBUGGING : 1
* PYDEVD_USE_FRAME_EVAL : NO
* PYTHONIOENCODING : utf-8
* PYTHONUNBUFFERED : 1
* PYTHON_FROZEN_MODULES : on
* SHELL : /bin/bash
* SHLVL : 2
* TERM : xterm-color
* USER : rduchadeau
* VSCODE_AMD_ENTRYPOINT : vs/workbench/api/node/extensionHostProcess
* VSCODE_CWD : /mnt/c/Users/romai/AppData/Local/Programs/Microsoft VS Code
* VSCODE_HANDLES_SIGPIPE : true
* VSCODE_HANDLES_UNCAUGHT_ERRORS : true
* VSCODE_IPC_HOOK_CLI : /run/user/1000/vscode-ipc-fba18183-d447-4a19-aea1-18bf6e42be3e.sock
* VSCODE_L10N_BUNDLE_LOCATION : 
* VSCODE_NLS_CONFIG : {"locale":"en","osLocale":"en","availableLanguages":{}}
* VSCODE_WSL_EXT_LOCATION : /mnt/c/Users/romai/.vscode/extensions/ms-vscode-remote.remote-wsl-0.88.2
* WAYLAND_DISPLAY : wayland-0
* WSL2_GUI_APPS_ENABLED : 1
* WSLENV : ELECTRON_RUN_AS_NODE/w:WT_SESSION:WT_PROFILE_ID:

* WSL_DISTRO_NAME : Ubuntu
* WSL_INTEROP : /run/WSL/45500_interop
* WT_PROFILE_ID : {51855cb2-8cce-5362-8f54-464b92b32386}
* WT_SESSION : bdf1dadb-b35e-46b2-9ab6-ce244d05b2de
* XDG_DATA_DIRS : /usr/local/share:/usr/share:/var/lib/snapd/desktop
* XDG_RUNTIME_DIR : /run/user/1000/
* _ : /home/rduchadeau/miniconda3/bin/python
* _CE_CONDA : 
* _CE_M : 

