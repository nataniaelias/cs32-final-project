# cs32-final-project
My CS32 Final Project w/ Eejenn, Lea, and Natania

Refined Description:
We are seeking to improve the popular scheduling tool When2Meet to offer a wider range of functionality, including potentially syncing with Google Calendar, having repeated time blocks, and incoporating preferences. To sync with the Google Calendar, we will use tools from Chapter 4 on querying to access GCAL and garner a response in JSON Format. For repeated time blocks and preferences, we will prompt the user to input whether their classes/extracurriculars/time commitments repeat and the range of willingness users have to meet at certain times. 

Larger processing steps: 
- add user option to select the range of meeting (Mon-Tues? 9-12am?)
- add user option to select the frequency of the meeting (weekly, daily, monthly?)
- add a user interface for indiating preferences (available, preferred, unpreferred) + store these preferences per time slot
- ensure time slots do not conflict with existing slots, especially those from Google Calendar
- ensure time slots optimize higher preference
- Import google calendar information + match to specific time slots


Specific examples of inputs and outputs, mainly the easiest to code first:
def create_event:
    #Description: This retrieves data from the user on the range of availability
    start_time = input ('Please pick the beginning of the time you will be available:')
    end_time = input ('Please pick the end of the time you will  be available:')
    
    slots = []
    # Description: This creates the time slots for the user
        while start_time <= end_time:
            slots.append(start_time)


Moving from this intital prototype to the final deliverable: Big picture, I want to refine the retrieval of data from the user by incoporating the preferences and Google Calendar component.
