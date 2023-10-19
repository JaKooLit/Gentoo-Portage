case "${EBUILD_PHASE}" in
        preinst) 
                DESC="${CATEGORY}/${PF}"
                NUMBER=`snapper create -t pre -p -d "${DESC}" -c number`
                ;;
        postinst) 
                snapper create -t post --pre-number $NUMBER -d "${DESC}" -c number
                ;;
esac
