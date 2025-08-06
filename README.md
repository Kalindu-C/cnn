## Image Classifier Using CNN

* ensure_annotations - stricly checked type of the function parameters
* ConfigBox - enable dictionary keys use as object's attributes
* created venv using uv package manager
* the files are genereating while axecution the program called artifacts


steps ->

1. update config.yml file
2. update params.yml
3. update entity



### Errors i'm encountered

error occured while execuitng training section which is exaclty here
 def get_base_model(self):
        self.model = tf.keras.models.load_model(
            self.config.updated_base_model_path
        )

        # Recompile the model with a fresh optimizer
        self.model.compile(
            optimizer=tf.keras.optimizers.Adam(self.config.params_learning_rate),
            loss='categorical_crossentropy',  # or 'binary_crossentropy' for binary classification
            metrics=['accuracy']
        )

initially there was no compile method and i added it now it's works


*** dagshub 

export MLFLOW_TRACKING_URI=https://dagshub.com/Kalindu-C/cnn.mlflow
export MLFLOW_TRACKING_USERNAME=Kalindu-C
export MLFLOW_TRACKING_PASSWORD=7974089bfe546160f38456c32264b8dda6073620
