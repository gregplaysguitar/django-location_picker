Provides a google maps location-picker widget for use in django forms,
and a complementary `LocationField` for django models, which uses the
widget by default in the django admin.


# Installation

1. Copy/symlink the location_picker module onto your path
2. If you're using staticfiles, add `'location_picker'` to your `INSTALLED_APPS` 
   setting.
3. If you're not using staticfiles, copy/symlink the 
   location_picker/static/location_picker directory into your static or media
   directory, and set `LOCATION_PICKER_STATIC_URL` appropriately.


# Usage

Use in your models.py as follows:
   
    from location_picker import LocationField
    
    class MyModel(models.Model):
        location = LocationField()

