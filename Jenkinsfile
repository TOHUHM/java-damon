    echo "Read values.yaml"
    def helm_value_data = readYaml file: './values.yaml'



    echo  "Update data values"

    try {

        helm_value_data.controller[tag_name].put('tag', "testtag")


    } catch (Exception err) {
        error(err.toString())
    }
