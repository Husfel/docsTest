MessageCheckingFailEventContent
================================

.. code-block:: c#

	class MessageCheckingFailEventContent {
		OutboxMessageMeta: OutboxMessageMeta,
		Errors: string[],
		ReportNumber: string
	}
	
Информация о новом событии - исходящее сообщение не прошло проверку на стороне получателя. Соответствует BoxEventType = MessageCheckingFail.

 - OutboxMessageMeta – :doc:`метаинформация <../../structures/OutboxMessageMeta>` проверенного сообщения.
 - Errors – ошибки, обнаруженные в сообщении, не прошедшем проверку.
 - ReportNumber – номер статусного сообщения, соответствующего данному событию. Актуален только для статусных отправляемых при схеме MetroOkNotOk.