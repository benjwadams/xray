.. currentmodule:: xray

#############
API reference
#############

This page provides an auto-generated summary of xray's API. For more details
and examples, refer to the relevant chapter in the main part of the
documentation.

Top-level functions
===================

.. autosummary::
   :toctree: generated/

   align
   concat

Dataset
=======

Creating a dataset
------------------

.. autosummary::
   :toctree: generated/

   Dataset
   decode_cf

Attributes
----------

.. autosummary::
   :toctree: generated/

   Dataset.dims
   Dataset.data_vars
   Dataset.coords
   Dataset.attrs

Dictionary interface
--------------------

Datasets implement the mapping interface with keys given by variable names
and values given by ``DataArray`` objects.

.. autosummary::
   :toctree: generated/

   Dataset.__getitem__
   Dataset.__setitem__
   Dataset.__delitem__
   Dataset.update
   Dataset.iteritems
   Dataset.itervalues

Dataset contents
----------------

.. autosummary::
   :toctree: generated/

   Dataset.copy
   Dataset.assign
   Dataset.assign_coords
   Dataset.merge
   Dataset.rename
   Dataset.swap_dims
   Dataset.drop
   Dataset.set_coords
   Dataset.reset_coords

Comparisons
-----------

.. autosummary::
   :toctree: generated/

   Dataset.equals
   Dataset.identical
   Dataset.broadcast_equals

Indexing
--------

.. autosummary::
   :toctree: generated/

   Dataset.loc
   Dataset.isel
   Dataset.sel
   Dataset.squeeze
   Dataset.reindex
   Dataset.reindex_like

Computation
-----------

.. autosummary::
   :toctree: generated/

   Dataset.apply
   Dataset.reduce
   Dataset.groupby
   Dataset.resample
   Dataset.transpose

**Aggregation**:
:py:attr:`~Dataset.all`
:py:attr:`~Dataset.any`
:py:attr:`~Dataset.argmax`
:py:attr:`~Dataset.argmin`
:py:attr:`~Dataset.max`
:py:attr:`~Dataset.mean`
:py:attr:`~Dataset.median`
:py:attr:`~Dataset.min`
:py:attr:`~Dataset.prod`
:py:attr:`~Dataset.sum`
:py:attr:`~Dataset.std`
:py:attr:`~Dataset.var`

**Missing values**:
:py:attr:`~Dataset.isnull`
:py:attr:`~Dataset.notnull`
:py:attr:`~Dataset.count`
:py:attr:`~Dataset.dropna`
:py:attr:`~Dataset.fillna`

**ndarray methods**:
:py:attr:`~Dataset.argsort`
:py:attr:`~Dataset.clip`
:py:attr:`~Dataset.conj`
:py:attr:`~Dataset.conjugate`
:py:attr:`~Dataset.round`
:py:attr:`~Dataset.T`

**Grouped operations**:
:py:attr:`~core.groupby.DatasetGroupBy.assign`
:py:attr:`~core.groupby.DatasetGroupBy.assign_coords`
:py:attr:`~core.groupby.DatasetGroupBy.first`
:py:attr:`~core.groupby.DatasetGroupBy.last`
:py:attr:`~core.groupby.DatasetGroupBy.fillna`

DataArray
=========

.. autosummary::
   :toctree: generated/

   DataArray

Attributes
----------

.. autosummary::
   :toctree: generated/

   DataArray.values
   DataArray.data
   DataArray.coords
   DataArray.dims
   DataArray.name
   DataArray.attrs
   DataArray.encoding

**ndarray attributes**:
:py:attr:`~DataArray.ndim`
:py:attr:`~DataArray.shape`
:py:attr:`~DataArray.size`
:py:attr:`~DataArray.dtype`

DataArray contents
------------------

.. autosummary::
   :toctree: generated/

   DataArray.assign_coords
   DataArray.rename
   DataArray.swap_dims
   DataArray.drop
   DataArray.reset_coords
   DataArray.copy

**ndarray methods**:
:py:attr:`~DataArray.astype`
:py:attr:`~DataArray.item`


Indexing
--------

.. autosummary::
   :toctree: generated/

   DataArray.__getitem__
   DataArray.__setitem__
   DataArray.loc
   DataArray.isel
   DataArray.sel
   DataArray.squeeze
   DataArray.reindex
   DataArray.reindex_like

Computation
-----------

.. autosummary::
   :toctree: generated/

   DataArray.reduce
   DataArray.groupby
   DataArray.resample
   DataArray.transpose
   DataArray.get_axis_num

**Aggregation**:
:py:attr:`~DataArray.all`
:py:attr:`~DataArray.any`
:py:attr:`~DataArray.argmax`
:py:attr:`~DataArray.argmin`
:py:attr:`~DataArray.max`
:py:attr:`~DataArray.mean`
:py:attr:`~DataArray.median`
:py:attr:`~DataArray.min`
:py:attr:`~DataArray.prod`
:py:attr:`~DataArray.sum`
:py:attr:`~DataArray.std`
:py:attr:`~DataArray.var`

**Missing values**:
:py:attr:`~DataArray.isnull`
:py:attr:`~DataArray.notnull`
:py:attr:`~DataArray.count`
:py:attr:`~DataArray.dropna`
:py:attr:`~DataArray.fillna`

**ndarray methods**:
:py:attr:`~DataArray.argsort`
:py:attr:`~DataArray.clip`
:py:attr:`~DataArray.conj`
:py:attr:`~DataArray.conjugate`
:py:attr:`~DataArray.searchsorted`
:py:attr:`~DataArray.round`
:py:attr:`~DataArray.T`

**Grouped operations**:
:py:attr:`~core.groupby.DataArrayGroupBy.assign_coords`
:py:attr:`~core.groupby.DataArrayGroupBy.first`
:py:attr:`~core.groupby.DataArrayGroupBy.last`
:py:attr:`~core.groupby.DataArrayGroupBy.fillna`

Comparisons
-----------

.. autosummary::
   :toctree: generated/

   DataArray.equals
   DataArray.identical
   DataArray.broadcast_equals

Universal functions
===================

This functions are copied from NumPy, but extended to work on NumPy arrays,
dask arrays and all xray objects. You can find them in the ``xray.ufuncs``
module:

:py:attr:`~ufuncs.angle`
:py:attr:`~ufuncs.arccos`
:py:attr:`~ufuncs.arccosh`
:py:attr:`~ufuncs.arcsin`
:py:attr:`~ufuncs.arcsinh`
:py:attr:`~ufuncs.arctan`
:py:attr:`~ufuncs.arctan2`
:py:attr:`~ufuncs.arctanh`
:py:attr:`~ufuncs.ceil`
:py:attr:`~ufuncs.conj`
:py:attr:`~ufuncs.copysign`
:py:attr:`~ufuncs.cos`
:py:attr:`~ufuncs.cosh`
:py:attr:`~ufuncs.deg2rad`
:py:attr:`~ufuncs.degrees`
:py:attr:`~ufuncs.exp`
:py:attr:`~ufuncs.expm1`
:py:attr:`~ufuncs.fabs`
:py:attr:`~ufuncs.fix`
:py:attr:`~ufuncs.floor`
:py:attr:`~ufuncs.fmax`
:py:attr:`~ufuncs.fmin`
:py:attr:`~ufuncs.fmod`
:py:attr:`~ufuncs.fmod`
:py:attr:`~ufuncs.frexp`
:py:attr:`~ufuncs.hypot`
:py:attr:`~ufuncs.imag`
:py:attr:`~ufuncs.iscomplex`
:py:attr:`~ufuncs.isfinite`
:py:attr:`~ufuncs.isinf`
:py:attr:`~ufuncs.isnan`
:py:attr:`~ufuncs.isreal`
:py:attr:`~ufuncs.ldexp`
:py:attr:`~ufuncs.log`
:py:attr:`~ufuncs.log10`
:py:attr:`~ufuncs.log1p`
:py:attr:`~ufuncs.log2`
:py:attr:`~ufuncs.logaddexp`
:py:attr:`~ufuncs.logaddexp2`
:py:attr:`~ufuncs.logical_and`
:py:attr:`~ufuncs.logical_not`
:py:attr:`~ufuncs.logical_or`
:py:attr:`~ufuncs.logical_xor`
:py:attr:`~ufuncs.maximum`
:py:attr:`~ufuncs.minimum`
:py:attr:`~ufuncs.nextafter`
:py:attr:`~ufuncs.rad2deg`
:py:attr:`~ufuncs.radians`
:py:attr:`~ufuncs.real`
:py:attr:`~ufuncs.rint`
:py:attr:`~ufuncs.sign`
:py:attr:`~ufuncs.signbit`
:py:attr:`~ufuncs.sin`
:py:attr:`~ufuncs.sinh`
:py:attr:`~ufuncs.sqrt`
:py:attr:`~ufuncs.square`
:py:attr:`~ufuncs.tan`
:py:attr:`~ufuncs.tanh`
:py:attr:`~ufuncs.trunc`

IO / Conversion
===============

Dataset methods
---------------

.. autosummary::
   :toctree: generated/

   open_dataset
   open_mfdataset
   Dataset.to_netcdf
   Dataset.to_dataframe
   Dataset.from_dataframe
   Dataset.close
   Dataset.load_data
   Dataset.reblock

DataArray methods
-----------------

.. autosummary::
   :toctree: generated/

   DataArray.to_dataset
   DataArray.to_pandas
   DataArray.to_series
   DataArray.to_dataframe
   DataArray.to_index
   DataArray.to_cdms2
   DataArray.from_series
   DataArray.from_cdms2
   DataArray.load_data
   DataArray.reblock

Backends (experimental)
-----------------------

These backends provide a low-level interface for lazily loading data from
external file-formats or protocols, and can be manually invoked to create
arguments for the ``from_store`` and ``dump_to_store`` Dataset methods.

.. autosummary::
   :toctree: generated/

   backends.NetCDF4DataStore
   backends.PydapDataStore
   backends.ScipyDataStore
