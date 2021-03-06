Change history
==============

1.4.4 (2020-03-25)

* Fix webargs 6.x.x: limit version < 6.

1.4.3 (2019-07-24)
******************

* Add CustomParser for automatically trim leading/trailing whitespace from argument values(`from hobbit_core.webargs import use_args, use_kwargs`).
* Add `HOBBIT_UPPER_SEQUENCE_NAME` config for upper db's sequence name.
* Fixs some err in template.

1.4.2 (2019-06-13)
******************

* Add `db.BaseModel` for support Oracle id sequence.

1.4.1 (2019-05-23)
******************

* Add template for 4-layers (view、schema、service、model).
* Add options api for query all consts defined in `app/models/consts`.
* Add `create` command to generate a csv file that defines some models to use in the `gen` command.
* Removed example code.
* Split hobbit cmd and hobbit_core lib, now install cmd should be `pip install "hobbit-core[hobbit,hobbit_core]"`.
* Remove flask_hobbit when import (`hobbit_core.flask_hobbit.db import transaction` --> `from hobbit_core.db import transaction`).
* Enhance gen cmd: now can auto create CRUD API and tests.
* Fix typo.
* Update some test cases.

1.4.0 (Obsolete version)
************************

1.3.1 (2019-02-26)
******************

* The strict parameter is removed in marshmallow >= 3.0.0.

1.3.0 (2019-01-14)
******************

* Add import_subs util for auto import models、schemas、views in module/__init__.py file.
* Add index for created_at、updated_at cloumn and default order_by id.
* Add validate for PageParams.
* Add hobbit gen cmd for auto render views.py, models.py, schemas.py etc when start a feature dev.
* Add ErrHandler.handler_assertion_error.
* Add db.transaction decorator, worked either autocommit True or False.
* pagination return dict instead of class, order_by can set None for
* traceback.print_exc() --> logging.error.
* Foreign key fields support ondelete, onupdate.
* Hobbit startproject cmd support celery option.

1.2.5 (2018-10-30)
******************

* Add ModelSchema(Auto generate load and dump func for EnumField).
* Add logging config file.
* Add EnumExt implementation.
* Fix use_kwargs with fileds.missing=None and enhanced.

1.2.4 (2018-10-18)
******************

* Fix SuccessResult status arg not used.

1.2.3 (2018-10-18)
******************

* Add utils.use_kwargs, fix webargs's bug.

1.2.2 (2018-10-16)
******************

* Add SchemaMixin & ORMSchema use in combination with db.SurrogatePK.
* Now print traceback info when server 500.
* Fix miss hidden files when sdist.

1.2.1 (2018-10-12)
******************

* secure_filename support py2 & py3.

1.2.0 (2018-10-11)
******************

* Gitlab CI/CD support.
* Add secure_filename util.
* Enhance deploy, can deploy to multiple servers.
* Add --port option for startproject cmd.

1.1.0 (2018-09-29)
******************

* Beta release.
* Fix hobbit create in curdir(.) err.
* Add dict2object util.
* Project tree confirmed.
* Add tutorial、project tree doc.
* Add example options for startproject cmd.


1.0.0 (2018-09-25)
******************

* Alpha release.
* flask_hobbit release.

0.0.[1-9]
*********

* hobbit cmd released.
* Incompatible production version.
