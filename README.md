valghalla cpr validator
=======================
Implements pluginsystem for cpr-validation of volunteers in valghalla.

How it works
------------
If activated, the module validates the volunteers PSN (cpr) in
hook_node_validate().

If address fetching is implemented in the plugin and activated address
information will be added to the volunteer node on hook_node_presave().

The callbacks defined in the plugin is called with the volunteers PSN as
a parameter.

Plugins
-------
A plugins can implement PSN validation and address fetching based
on the volunteers PSN. As well as a configuration page for the plugin
itself.

###Example
See modules/valghalla_cpr_service_dummy for implementation details for
plugins.

Licence and copyright
---------------------
Valghalla is Copyright (c) 2012 OS2 - Offentligt Digitaliseringsfællesskab,
Denmark <http://os2web.dk/>

Valghalla is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

Valghalla is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
ERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
