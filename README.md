MWDatePicker
============

Great flat date picker for iOS

Simply use as the following:
	MWDatePicker *picker = [[MWDatePicker alloc] initWithPickerMode:mwDatePickerModeDateTime];
	picker.title = @"Start Date";
	picker.delegate = self;
	[picker presentInView:self.view];

The delegate protocol is the following:
	-(void)mwDatePicker:(MWDatePicker *)picker didChangeDate:(NSDate *)date;
	-(void)mwDatePickerDidCancel:(MWDatePicker *)picker;
	-(void)mwDatePickerDidFinish:(MWDatePicker *)picker;

If you would rather use blocks, that's available as well
	[picker setHandlerForDateChange:^(NSDate *date) {
	
	}];

	[picker setHandlerForCancel:^{

	}];

	[picker setHandlerForFinish:^{

	}];